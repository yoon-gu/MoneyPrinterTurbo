# 2026-04-02 PR 병합 및 검증 기록

## 이번에 병합하고 푸시한 PR

- `#837` `fix: update google-generativeai version for response_modalities support`
- `#835` `fix: add missing pydub dependency to requirements.txt`
- `#850` `feat: support reading subtitle position from config file`
- `#838` `feat: add MiniMax as LLM provider`
- `#811` `refactor: optimize codebase for better performance and reliability`
- `#848` `feat: support GPU acceleration for faster-whisper in Docker`
- `#843` `feat: Add Upload-Post integration for cross-posting to TikTok/Instagram`

## 병합 후 메인 브랜치 커밋

- TTS 및 자막 수정 기준 커밋: `953a6c0` `fix: restore edge tts synthesis and readable subtitles`
- 현재 메인 브랜치 커밋: `1f8a746`

## 병합 시 검증 결과

### 통과

- `#837`
  - 의존성 업그레이드 후 정상적으로 import됨
  - `google-generativeai==0.8.6` 적용 확인
- `#835`
  - `pydub==0.25.1` 적용 확인
- `#850`
  - `subtitle_position`과 `custom_position`을 설정 파일에서 읽을 수 있음
- `#838`
  - MiniMax provider 연결 정상
  - mock 호출로 `_generate_response` 통과 검증
- `#811`
  - 메인 브랜치 import 정상
  - 샘플 단위 테스트 통과
- `#848`
  - `docker compose -f docker-compose.yml -f docker-compose.gpu.yml config` 정상 파싱
- `#843`
  - Upload-Post 서비스 import 및 mock 업로드 호출 통과
  - 앞선 PR들과 함께 적용할 때 `config.example.toml` 설정 구간에서만 충돌이 있었고, 양쪽 내용을 수동으로 보존함

### 거절 및 종료

- `#852`
  - 오디오는 복구할 수 있지만 자막 흐름을 깨고 WebUI에서 여전히 호출하는 Gemini 로직을 삭제함
- `#787`
  - 현재 `403` 상황을 해결하지 못함
- `#841`
  - 현재 메인 브랜치의 TTS/자막 수정과 충돌하며, 더 작은 PR이 이미 동일한 이득을 제공함
- `#824`
  - ModelsLab 경로는 오디오를 생성할 수 있지만 자막 흐름이 실패해 사용 가능한 SRT를 만들 수 없음
- `#840`
  - 백엔드에 `video_source="ai"`를 추가했지만 WebUI가 해당 값을 아직 지원하지 않아 엔드투엔드로 사용할 수 없음
- `#826`
  - 현재 메인 브랜치의 `voice.py` 및 의존성 변경과 충돌해 병합 검증을 통과하지 못함
- `#751`
- `#749`
- `#742`
- `#705`
  - 위 4개 PR은 현재 메인 브랜치 기준 모두 `DIRTY` 상태이며 병합 검증을 통과하지 못함

## 스모크 테스트 기록

### 서비스 재시작

- API: `http://127.0.0.1:8080/docs`
- WebUI: `http://127.0.0.1:8501`

### 첫 번째 전체 영상 작업

- 작업 ID: `ced0b190-dd72-489c-b978-2761740933db`
- 결과: 실패
- 결론:
  - API 기본값이 `video_transition_mode=null`
  - 영상 이어붙이기 단계에서 `app/services/video.py`가 `video_transition_mode.value`에 직접 접근함
  - 이로 인해 작업 스레드가 예외로 종료되고 작업 상태가 `state=4, progress=75`에 머무름

### 두 번째 전체 영상 작업

- 작업 ID: `8b2a0e6e-b3e6-44ab-a1b4-1865a0b4788d`
- 제출 방식:
  - `POST /api/v1/videos`
  - 로컬 소재 `/Users/harry/Projects/Python/MoneyPrinterTurbo/test/resources/1.png` 사용
  - `video_transition_mode="FadeIn"`을 명시적으로 지정
- 결과: 성공
- 작업 상태: `state=1, progress=100`

### 두 번째 작업 산출물

- 오디오: `/Users/harry/Projects/Python/MoneyPrinterTurbo/storage/tasks/8b2a0e6e-b3e6-44ab-a1b4-1865a0b4788d/audio.mp3`
  - 길이: `8.952s`
  - 크기: `53712 bytes`
- 이어붙인 영상: `/Users/harry/Projects/Python/MoneyPrinterTurbo/storage/tasks/8b2a0e6e-b3e6-44ab-a1b4-1865a0b4788d/combined-1.mp4`
  - 길이: `9.000s`
  - 크기: `177666 bytes`
- 최종 영상: `/Users/harry/Projects/Python/MoneyPrinterTurbo/storage/tasks/8b2a0e6e-b3e6-44ab-a1b4-1865a0b4788d/final-1.mp4`
  - 길이: `9.000s`
  - 크기: `352810 bytes`
- 자막: `/Users/harry/Projects/Python/MoneyPrinterTurbo/storage/tasks/8b2a0e6e-b3e6-44ab-a1b4-1865a0b4788d/subtitle.srt`

### 두 번째 작업 자막 샘플

```srt
1
00:00:00,100 --> 00:00:03,300
메인 브랜치 병합 후 진행한 전체 스모크 테스트입니다

2
00:00:03,875 --> 00:00:05,350
음성

3
00:00:05,575 --> 00:00:08,375
자막과 최종 영상이 모두 정상적으로 생성되는지 확인합니다
```

## 현재 주의해야 할 위험

- `#843`은 mock 검증만 수행했으며 실제 Upload-Post 키로 연동 테스트하지 않았음
- `#848`은 Docker GPU 설정 파싱만 검증했으며 실제 GPU 환경에서 실행하지 않았음
- 현재 API 기본값 `video_transition_mode=null`일 때 전체 영상 작업에 여전히 회귀 위험이 있음
