<div align="center">
<h1 align="center">MoneyPrinterTurbo 💸</h1>

<p align="center">
  <a href="https://github.com/harry0703/MoneyPrinterTurbo/stargazers"><img src="https://img.shields.io/github/stars/harry0703/MoneyPrinterTurbo.svg?style=for-the-badge" alt="Stargazers"></a>
  <a href="https://github.com/harry0703/MoneyPrinterTurbo/issues"><img src="https://img.shields.io/github/issues/harry0703/MoneyPrinterTurbo.svg?style=for-the-badge" alt="Issues"></a>
  <a href="https://github.com/harry0703/MoneyPrinterTurbo/network/members"><img src="https://img.shields.io/github/forks/harry0703/MoneyPrinterTurbo.svg?style=for-the-badge" alt="Forks"></a>
  <a href="https://github.com/harry0703/MoneyPrinterTurbo/blob/main/LICENSE"><img src="https://img.shields.io/github/license/harry0703/MoneyPrinterTurbo.svg?style=for-the-badge" alt="License"></a>
</p>
<br>
<h3>한국어 | <a href="README-en.md">English</a></h3>
<div align="center">
  <a href="https://trendshift.io/repositories/8731" target="_blank"><img src="https://trendshift.io/api/badge/repositories/8731" alt="harry0703%2FMoneyPrinterTurbo | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
</div>
<br>
영상 <b>주제</b> 또는 <b>키워드</b>만 입력하면 영상 문안, 영상 소재, 자막, 배경 음악을 자동으로 생성하고 HD 숏폼 영상으로 합성합니다.
<br>

<h4>Web 인터페이스</h4>

![](docs/webui.jpg)

<h4>API 인터페이스</h4>

![](docs/api.jpg)

</div>

## 주요 기능 🎯

- [x] 완전한 **MVC 아키텍처**와 명확한 코드 구조로 유지보수가 쉽고 `API`와 `Web 인터페이스`를 모두 지원합니다.
- [x] 영상 문안을 **AI로 자동 생성**하거나 **직접 입력**할 수 있습니다.
- [x] 여러 **HD 영상** 크기를 지원합니다.
    - [x] 세로 9:16, `1080x1920`
    - [x] 가로 16:9, `1920x1080`
- [x] **일괄 영상 생성**을 지원하여 여러 영상을 한 번에 만들고 가장 마음에 드는 결과를 선택할 수 있습니다.
- [x] **영상 클립 길이**를 설정하여 소재 전환 빈도를 조절할 수 있습니다.
- [x] **한국어**, **중국어**, **영어** 등 여러 언어의 영상 문안을 지원합니다.
- [x] **다양한 음성** 합성을 지원하며 결과를 **실시간으로 미리듣기**할 수 있습니다.
- [x] **자막 생성**을 지원하며 `글꼴`, `위치`, `색상`, `크기`, `자막 외곽선`을 조정할 수 있습니다.
- [x] **배경 음악**을 랜덤으로 선택하거나 특정 음악 파일을 지정할 수 있으며 `배경 음악 음량`도 설정할 수 있습니다.
- [x] 영상 소재는 **HD** 및 **저작권 프리** 소스를 사용하며, 사용자의 **로컬 소재**도 사용할 수 있습니다.
- [x] **OpenAI**, **Moonshot**, **Azure**, **gpt4free**, **one-api**, **Qwen**, **Google Gemini**, **Ollama**, **DeepSeek**, **MiniMax**, **ERNIE**, **Pollinations**, **ModelScope** 등 다양한 모델 연동을 지원합니다.

## 영상 데모 📺

### 세로 9:16

<table>
<thead>
<tr>
<th align="center"><g-emoji class="g-emoji" alias="arrow_forward">▶️</g-emoji> 《삶의 즐거움을 늘리는 방법》</th>
<th align="center"><g-emoji class="g-emoji" alias="arrow_forward">▶️</g-emoji> 《돈의 역할》<br>더 자연스러운 합성 음성</th>
<th align="center"><g-emoji class="g-emoji" alias="arrow_forward">▶️</g-emoji> 《삶의 의미는 무엇인가》</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center"><video src="https://github.com/harry0703/MoneyPrinterTurbo/assets/4928832/a84d33d5-27a2-4aba-8fd0-9fb2bd91c6a6"></video></td>
<td align="center"><video src="https://github.com/harry0703/MoneyPrinterTurbo/assets/4928832/af2f3b0b-002e-49fe-b161-18ba91c055e8"></video></td>
<td align="center"><video src="https://github.com/harry0703/MoneyPrinterTurbo/assets/4928832/112c9564-d52b-4472-99ad-970b75f66476"></video></td>
</tr>
</tbody>
</table>

### 가로 16:9

<table>
<thead>
<tr>
<th align="center"><g-emoji class="g-emoji" alias="arrow_forward">▶️</g-emoji>《삶의 의미는 무엇인가》</th>
<th align="center"><g-emoji class="g-emoji" alias="arrow_forward">▶️</g-emoji>《왜 운동해야 할까》</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center"><video src="https://github.com/harry0703/MoneyPrinterTurbo/assets/4928832/346ebb15-c55f-47a9-a653-114f08bb8073"></video></td>
<td align="center"><video src="https://github.com/harry0703/MoneyPrinterTurbo/assets/4928832/271f2fae-8283-44a0-8aa0-0ed8f9a6fa87"></video></td>
</tr>
</tbody>
</table>

## 요구 사양 📦

- 권장 시스템: Windows 10 이상, macOS 11.0 이상, 또는 주요 Linux 배포판
- GPU는 필수는 아니지만 로컬 전사, 더 빠른 영상 처리, 더 원활한 일괄 생성이 필요하다면 전용 그래픽카드를 권장합니다.

| 항목 | 최소 사양 | 권장 사양 | 이상적 사양 |
| --- | --- | --- | --- |
| CPU | 4코어 | 6-8코어 | 8코어 이상 |
| RAM | 4 GB | 8 GB | 16 GB 이상 |
| GPU | 필수 아님 | VRAM 4 GB 이상 | VRAM 8 GB 이상 |

- 클라우드 LLM, 클라우드 TTS, 온라인 소재 소스를 주로 사용한다면 GPU보다 CPU와 메모리가 더 중요합니다.
- `faster-whisper`, 일괄 생성, 무거운 로컬 처리 흐름을 사용하면 GPU가 속도를 크게 높여 줍니다.

## 빠른 시작 🚀

### 권장 사용 방식

- Windows 사용자: 빠른 체험에는 원클릭 실행 패키지를 우선 사용하세요.
- macOS / Linux 사용자: `uv sync --frozen` 기반 로컬 배포를 우선 권장합니다.
- 격리된 실행 환경이 필요하다면 Docker 배포를 권장합니다.

### Google Colab에서 실행

로컬 환경 설정 없이 Google Colab에서 바로 MoneyPrinterTurbo를 체험할 수 있습니다.

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/harry0703/MoneyPrinterTurbo/blob/main/docs/MoneyPrinterTurbo.ipynb)

### Windows 원클릭 실행 패키지

원클릭 실행 패키지를 내려받아 압축을 풀고 바로 사용할 수 있습니다. 경로에는 **중국어**, **특수 문자**, **공백**을 넣지 않는 것을 권장합니다.
현재 제공되는 설치 패키지는 아직 `v1.2.6`의 이전 패키징 버전입니다. 다운로드 후 먼저 `update.bat`을 실행해 최신 코드로 업데이트하는 것을 권장합니다.

- Baidu Netdisk(v1.2.6): https://pan.baidu.com/s/1wg0UaIyXpO3SqIpaq790SQ?pwd=sbqx 추출 코드: sbqx
- Google Drive(v1.2.6): https://drive.google.com/file/d/1HsbzfT7XunkrCrHw5ncUjFX8XX4zAuUh/view?usp=sharing

다운로드 후 `update.bat`을 **더블 클릭하여** 최신 코드로 업데이트한 다음 `start.bat`을 더블 클릭해 시작하세요.

시작하면 브라우저가 자동으로 열립니다. 빈 화면이 표시되면 **Chrome** 또는 **Edge**로 열어 보세요.

## 설치 및 배포 📥

### 전제 조건

- 예기치 못한 문제를 피하려면 **중국어 경로**를 가능한 한 사용하지 마세요.
- **네트워크**가 정상인지 확인하세요. VPN이 필요하다면 `전체 트래픽` 모드로 설정하세요.

#### ① 코드 클론

```shell
git clone https://github.com/harry0703/MoneyPrinterTurbo.git
```

#### ② 설정 파일 수정(선택, WebUI 시작 후 설정해도 됨)

- `config.example.toml` 파일을 복사해 `config.toml`로 이름을 바꿉니다.
- `config.toml` 설명에 따라 `pexels_api_keys`와 `llm_provider`를 설정하고, 선택한 llm_provider에 맞는 API Key를 입력합니다.

### Docker 배포 🐳

#### ① Docker 시작

Docker가 설치되어 있지 않다면 https://www.docker.com/products/docker-desktop/ 에서 먼저 설치하세요.

Windows라면 Microsoft 문서를 참고하세요.

1. https://learn.microsoft.com/zh-cn/windows/wsl/install
2. https://learn.microsoft.com/zh-cn/windows/wsl/tutorials/wsl-containers

```shell
cd MoneyPrinterTurbo
docker-compose up
```

> 참고: 최신 Docker는 설치 시 docker compose를 플러그인 형태로 함께 설치하므로 실행 명령은 `docker compose up`으로 조정할 수 있습니다.

#### ② Web 인터페이스 접속

브라우저에서 http://127.0.0.1:8501 로 접속합니다.

#### ③ API 문서 접속

브라우저에서 http://0.0.0.0:8080/docs 또는 http://0.0.0.0:8080/redoc 으로 접속합니다.

### 수동 배포 📦

> 영상 튜토리얼

- 전체 사용 데모: https://v.douyin.com/iFhnwsKY/
- Windows 배포 방법: https://v.douyin.com/iFyjoW3M

#### ① 가상 환경 생성

Python 환경과 의존성 관리는 [uv](https://docs.astral.sh/uv/) 사용을 권장합니다. 기본 Python 버전은 `3.11`입니다.

```shell
git clone https://github.com/harry0703/MoneyPrinterTurbo.git
cd MoneyPrinterTurbo
uv python install 3.11
uv sync --frozen
```

`uv`를 사용하지 않는다면 `venv + pip` 방식도 계속 사용할 수 있습니다.

```shell
python3.11 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

설명:
- `pyproject.toml`은 주요 의존성 정의 파일입니다.
- `uv.lock`은 잠금 파일이며 기본적으로 `uv sync --frozen` 실행을 권장합니다.
- `requirements.txt`는 기존 `pip` 설치 방식과의 호환을 위해 유지됩니다.

#### ② ImageMagick 설치

- Windows:
    - https://imagemagick.org/script/download.php 에서 Windows 버전을 다운로드하되 반드시 **static** 버전을 선택하세요. 예: ImageMagick-7.1.1-32-Q16-x64-**static**.exe
    - 다운로드한 ImageMagick을 설치합니다. **설치 경로는 변경하지 않는 것을 권장합니다.**
    - `config.toml` 설정 파일의 `imagemagick_path`를 **실제 설치 경로**로 수정합니다.

- macOS:
  ```shell
  brew install imagemagick
  ````
- Ubuntu:
  ```shell
  sudo apt-get install imagemagick
  ```
- CentOS:
  ```shell
  sudo yum install ImageMagick
  ```

#### ③ Web 인터페이스 시작 🌐

아래 명령은 MoneyPrinterTurbo 프로젝트 `루트 디렉터리`에서 실행해야 합니다.

###### Windows

```powershell
.\webui.bat
```

CMD에서도 `webui.bat`을 실행할 수 있습니다.
`webui.bat`은 프로젝트 `.venv` 또는 원클릭 패키지에 포함된 Python을 우선 사용합니다. 프로젝트 Python을 찾지 못했지만 `uv`가 설치되어 있으면 자동으로 `uv run streamlit`으로 전환합니다.
LAN의 다른 장치에서 WebUI에 접근하도록 허용하려면 먼저 `set MPT_WEBUI_HOST=0.0.0.0`을 실행한 뒤 `webui.bat`을 실행하세요.

###### macOS 또는 Linux

```shell
uv run streamlit run ./webui/Main.py --browser.gatherUsageStats=False
```

가상 환경을 이미 수동으로 활성화했다면 아래 명령을 직접 실행할 수도 있습니다.

```shell
sh webui.sh
```

시작하면 브라우저가 자동으로 열립니다. 빈 화면이 표시되면 **Chrome** 또는 **Edge**로 열어 보세요.

#### ④ API 서비스 시작 🚀

```shell
uv run python main.py
```

가상 환경을 이미 수동으로 활성화했다면 아래 명령을 직접 실행할 수도 있습니다.

```shell
python main.py
```

## 특별 감사 🙏

이 프로젝트의 **배포**와 **사용**은 초보 사용자에게 어느 정도 진입 장벽이 있습니다. 이 프로젝트를 기반으로 무료 `AI 영상 생성기` 서비스를 제공해 별도 배포 없이 온라인에서 편리하게 사용할 수 있도록 한 **RecCloud(AI 지능형 멀티미디어 서비스 플랫폼)**에 감사드립니다.

- 중국어 버전: https://reccloud.cn
- 영어 버전: https://reccloud.com

![](docs/reccloud.cn.jpg)

## 후원 감사 🙏

이 프로젝트가 지속적으로 업데이트되고 유지보수될 수 있도록 지원해 준 PicWish https://picwish.cn 에 감사드립니다.

PicWish는 **이미지 처리 분야**에 집중하며 다양한 **이미지 처리 도구**를 제공해 복잡한 작업을 단순화하고 이미지 처리를 더 쉽게 만들어 줍니다.

![picwish.jpg](docs/picwish.jpg)

시작 후 `API 문서` http://127.0.0.1:8080/docs 또는 http://127.0.0.1:8080/redoc 에서 인터페이스를 온라인으로 직접 테스트할 수 있습니다.

## 음성 합성 🗣

지원되는 모든 음성 목록은 [음성 목록](./docs/voice-list.txt)에서 확인할 수 있습니다.

2024-04-16 v1.1.2에서 Azure 음성 합성 음성 9종이 추가되었습니다. API KEY 설정이 필요하며 더 자연스러운 음성 합성이 가능합니다.

## 자막 생성 📜

현재 2가지 자막 생성 방식을 지원합니다.

- **edge**: 생성 `속도가 빠르고` 성능이 좋으며 컴퓨터 사양 요구가 낮지만 품질이 불안정할 수 있습니다.
- **whisper**: 생성 `속도가 느리고` 성능 부담이 더 크며 컴퓨터 사양 요구가 있지만 `품질이 더 안정적`입니다.

`config.toml` 설정 파일의 `subtitle_provider`를 수정해 전환할 수 있습니다.

먼저 `edge` 모드를 사용하고, 자막 품질이 좋지 않다면 `whisper` 모드로 전환하는 것을 권장합니다.

> 참고:

1. whisper 모드에서는 HuggingFace에서 약 3GB 크기의 모델 파일을 다운로드해야 하므로 네트워크 상태를 확인하세요.
2. 값을 비워 두면 자막을 생성하지 않습니다.

> HuggingFace에 접근하기 어려운 환경이라면 아래 방법으로 `whisper-large-v3` 모델 파일을 수동 다운로드할 수 있습니다.

다운로드 주소:

- Baidu Netdisk: https://pan.baidu.com/s/11h3Q6tsDtjQKTjUu3sc5cA?pwd=xjs9
- Quark Netdisk: https://pan.quark.cn/s/3ee3d991d64b

모델을 다운로드해 압축을 푼 뒤 전체 디렉터리를 `.\MoneyPrinterTurbo\models` 안에 넣습니다.
최종 파일 경로는 다음과 같아야 합니다: `.\MoneyPrinterTurbo\models\whisper-large-v3`

```
MoneyPrinterTurbo
  ├─models
  │   └─whisper-large-v3
  │          config.json
  │          model.bin
  │          preprocessor_config.json
  │          tokenizer.json
  │          vocabulary.json
```

## 배경 음악 🎵

영상에 사용하는 배경 음악은 프로젝트의 `resource/songs` 디렉터리에 있습니다.
> 현재 프로젝트에는 YouTube 영상에서 가져온 기본 음악이 일부 포함되어 있습니다. 권리 문제가 있다면 삭제하세요.

## 자막 글꼴 🅰

영상 자막 렌더링에 사용하는 글꼴은 프로젝트의 `resource/fonts` 디렉터리에 있습니다. 직접 준비한 글꼴을 넣어 사용할 수도 있습니다.

## 자주 묻는 질문 🤔

### ❓RuntimeError: No ffmpeg exe could be found

일반적으로 ffmpeg는 자동으로 다운로드되고 자동 감지됩니다.
하지만 환경 문제로 자동 다운로드가 불가능하면 아래 오류가 발생할 수 있습니다.

```
RuntimeError: No ffmpeg exe could be found.
Install ffmpeg on your system, or set the IMAGEIO_FFMPEG_EXE environment variable.
```

이 경우 https://www.gyan.dev/ffmpeg/builds/ 에서 ffmpeg를 다운로드해 압축을 풀고 `ffmpeg_path`를 실제 설치 경로로 설정하세요.

```toml
[app]
# 실제 경로에 맞게 설정하세요. Windows 경로 구분자는 \\ 입니다.
ffmpeg_path = "C:\\Users\\harry\\Downloads\\ffmpeg.exe"
```

### ❓ImageMagick의 보안 정책이 임시 파일 @/tmp/tmpur5hyyto.txt 관련 작업을 차단함

ImageMagick의 `policy.xml` 설정 파일에서 해당 정책을 찾을 수 있습니다.
이 파일은 보통 `/etc/ImageMagick-X/` 또는 ImageMagick 설치 디렉터리의 유사한 위치에 있습니다.
`pattern="@"`가 포함된 항목을 찾아 `rights="none"`을 `rights="read|write"`로 변경하면 파일 읽기/쓰기 작업이 허용됩니다.

### ❓OSError: [Errno 24] Too many open files

시스템의 열린 파일 수 제한 때문에 발생하는 문제입니다. 파일 열기 제한을 조정해 해결할 수 있습니다.

현재 제한 확인:

```shell
ulimit -n
```

값이 너무 낮다면 예를 들어 다음처럼 높일 수 있습니다.

```shell
ulimit -n 10240
```

### ❓Whisper 모델 다운로드 실패와 아래 오류

LocalEntryNotfoundEror: Cannot find an appropriate cached snapshotfolderfor the specified revision on the local disk and
outgoing trafic has been disabled.
To enablerepo look-ups and downloads online, pass 'local files only=False' as input.

또는

An error occurred while synchronizing the model Systran/faster-whisper-large-v3 from the Hugging Face Hub:
An error happened while trying to locate the files on the Hub and we cannot find the appropriate snapshot folder for the
specified revision on the local disk. Please check your internet connection and try again.
Trying to load the model directly from the local cache, if it exists.

해결 방법: [모델을 수동 다운로드하는 방법 보기](#자막-생성-)

## 피드백 및 제안 📢

- [issue](https://github.com/harry0703/MoneyPrinterTurbo/issues) 또는 [pull request](https://github.com/harry0703/MoneyPrinterTurbo/pulls)를 제출할 수 있습니다.

## 라이선스 📝

[`LICENSE`](LICENSE) 파일을 확인하세요.

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=harry0703/MoneyPrinterTurbo&type=Date)](https://star-history.com/#harry0703/MoneyPrinterTurbo&Date)
