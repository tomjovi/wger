# wger

🌍 [English](README.md) | **한국어**

<p align="center">
  <img src="https://raw.githubusercontent.com/wger-project/wger/master/wger/core/static/images/logos/logo.png" width="100" height="100" alt="wger 로고">

![AGPLv3 License](https://img.shields.io/badge/License-AGPLv3-blue.svg)
![Build Status](https://img.shields.io/github/actions/workflow/status/wger-project/wger/ci.yml?branch=master)
[![Coverage Status](https://coveralls.io/repos/github/wger-project/wger/badge.svg?branch=master)](https://coveralls.io/github/wger-project/wger?branch=master)
![Translation Status](https://hosted.weblate.org/widget/wger/svg-badge.svg)
</p>

wger (ˈvɛɡɐ, "베거"라고 발음)는 무료 운동 및 피트니스 관리 프로그램입니다.

- 🏋️ **맞춤 운동 루틴** – 자동 중량 증가 규칙이 적용되는 유연한 루틴을 만들 수 있습니다.
- 📊 **종합적인 기록** – 식단 계획, 체중, 사용자 정의 측정 항목을 추적합니다.
- 🍽️ **영양 관리** – [Open Food Facts](https://openfoodfacts.org)의 식품 데이터베이스로 칼로리를 기록합니다.
- 📸 **progress gallery(성장 갤러리)** – 운동 전후 사진을 업로드하고 신체 변화를 추적합니다.
- 📚 **운동 위키** – 내장된 운동 동작 사전(위키)을 이용하고 직접 기여할 수도 있습니다.
- 📱 **크로스 플랫폼 앱** –
  [Android](https://play.google.com/store/apps/details?id=de.wger.flutter),
  [iOS](https://apps.apple.com/us/app/wger-workout-manager/id6502226792),
  [F-Droid](https://f-droid.org/en/packages/de.wger.flutter/),
  [Flathub](https://flathub.org/apps/de.wger.flutter)에서 사용할 수 있습니다.
- 🐳 **셀프 호스팅** – Docker로 간편하게 직접 서버에 설치해 모든 데이터를 직접 관리할 수 있습니다.
- 🌍 **다국어 지원** – Weblate를 통한 커뮤니티 번역으로 여러 언어를 지원합니다.
- 🔗 **강력한 API** – 서드파티 연동이나 자동화를 위한 REST API를 제공합니다.
- 👥 **다중 사용자 지원** – 기본적인 헬스장(짐) 관리 기능을 포함합니다.
- 🆓 **100% 무료 & 오픈소스** – AGPL-3.0 또는 그 이후 버전 라이선스입니다.

실제로 동작하는 사이트를 사용해 보려면 <https://wger.de> 를 방문하세요.

<p align="center" style="line-height:0; margin:0; padding:0;">
  <a href="https://play.google.com/store/apps/details?id=de.wger.flutter" target="_blank" style="text-decoration:none; border:none; outline:none;"><img src="https://raw.githubusercontent.com/wger-project/wger/master/wger/core/static/images/logos/play-store/badge.svg" alt="Google Play에서 받기" height="50" style="margin-right:8px; vertical-align:middle; border:none; outline:none; display:inline-block;"></a>
  <a href="https://apps.apple.com/us/app/wger-workout-manager/id6502226792" target="_blank" style="text-decoration:none; border:none; outline:none;"><img src="https://developer.apple.com/assets/elements/badges/download-on-the-app-store.svg" alt="App Store에서 다운로드" height="64" style="margin-right:8px; vertical-align:middle; border:none; outline:none; display:inline-block; background:none;"></a>
  <a href="https://f-droid.org/packages/de.wger.flutter/" target="_blank" style="text-decoration:none; border:none; outline:none;"><img src="https://raw.githubusercontent.com/wger-project/wger/master/wger/core/static/images/logos/fdroid/get-it-on.png" alt="F-Droid에서 받기" height="50" style="margin-right:8px; vertical-align:middle; border:none; outline:none; display:inline-block; background:none;"></a>
  <a href="https://flathub.org/apps/de.wger.flutter" target="_blank" style="text-decoration:none; border:none; outline:none;"><img src="https://raw.githubusercontent.com/wger-project/wger/master/wger/core/static/images/logos/flathub/black.svg" alt="Flathub에서 받기" height="50" style="vertical-align:middle; border:none; outline:none; display:inline-block; background:none;"></a>
</p>

## 사용 방법

wger는 크게 3가지 방법으로 사용할 수 있습니다.

### 1. 공식 서버 / 앱 그대로 사용하기 (가장 쉬움)

설치 없이 바로 운동 관리를 시작하고 싶다면 이 방법이 가장 좋습니다.

1. 웹 브라우저로 <https://wger.de> 에 접속해 회원가입합니다.
2. 스마트폰에서는 아래 앱을 설치하고 `wger.de` 계정(또는 본인 서버 주소)으로 로그인합니다.
   - [Android (Google Play)](https://play.google.com/store/apps/details?id=de.wger.flutter)
   - [iOS (App Store)](https://apps.apple.com/us/app/wger-workout-manager/id6502226792)
   - [F-Droid](https://f-droid.org/en/packages/de.wger.flutter/)
   - [Flathub (리눅스 데스크톱)](https://flathub.org/apps/de.wger.flutter)
3. 웹 또는 앱에서 운동 루틴 만들기 → 운동 기록 → 체중·식단 기록 순서로 사용하면 됩니다.

### 2. Docker로 직접 호스팅하기 (셀프 호스팅)

내 서버에 직접 설치하면 모든 데이터를 내가 소유하고, 가족·회원과 함께 쓸 수 있습니다.
기본적으로 `docker compose up -d` 한 줄이면 실행됩니다.

```bash
# 1. 공식 compose 파일 내려받기
git clone https://github.com/wger-project/docker wger-docker
cd wger-docker

# 2. 백그라운드로 실행
docker compose up -d
```

그 뒤 브라우저에서 `http://localhost` (또는 서버 주소)로 접속하면 됩니다.
자세한 설정(도메인, HTTPS, 이메일, 백업 등)은 아래 문서를 참고하세요.

- compose 파일: [wger-project/docker](https://github.com/wger-project/docker)
- 설치 문서: [wger.readthedocs.io 설치 가이드](https://wger.readthedocs.io/en/latest/installation/docker.html)

> 간단히 체험만 해보고 싶다면 데모 이미지도 있습니다.
>
> ```bash
> docker run -ti --name wger.demo --publish 8000:80 wger/demo
> ```
>
> 이후 <http://localhost:8000> 에 접속해 `admin` / `adminadmin` 으로 로그인하세요.
> 단, 데모 이미지는 업데이트 시 데이터가 초기화되므로 실제 기록용으로는 사용하지 마세요.

### 3. 개발용으로 실행하기 (기여·커스텀용)

코드를 수정하거나 기여하고 싶다면 개발 환경으로 실행하세요.

```bash
git clone https://github.com/wger-project/wger.git
cd wger
# 개발용 docker 설정 참고:
# extras/docker/development/README.md
docker compose up
```

자세한 개발·기여 절차는 아래 [개발 및 기여](#개발-및-기여) 섹션과
[기여 가이드](https://wger.readthedocs.io/en/latest/contributing.html)를 참고하세요.

## 셀프 호스팅

직접 서버를 운영하는 것은 기본적으로 `docker compose up -d` 한 줄이면 됩니다.
자세한 설치 방법은 함께 제공되는
[docker compose 파일](https://github.com/wger-project/docker)과
[관련 문서](https://wger.readthedocs.io/en/latest/installation/docker.html)를
참고하세요.

## 개발 및 기여

우리의 목표는 멋지고 유연한 피트니스·영양 관리자를 만들고, 운동과 식재료 목록을
자유 라이선스로 함께 구축하는 것입니다.

이를 위해 여러분의 도움이 필요합니다! 코드, 번역, 운동 데이터 작성, 이슈·아이디어
제보 등 어떤 기여든 환영합니다. 먼저
[기여 가이드](https://wger.readthedocs.io/en/latest/contributing.html)를
확인하고 시작해 보세요.

지금까지 기여해 주신 모든 분들께 진심으로 감사드립니다! ❤️ 전체 명단은
[AUTHORS.md](AUTHORS.md)에서 확인할 수 있습니다.

## 문서

온라인 문서를 참고하세요.

* <https://wger.readthedocs.io>

설치 방법, API 문서, 개발 가이드 등의 정보를 확인할 수 있습니다.

## 문의

유용하게 사용하셨거나, 예상과 다르게 동작하는 부분이 있다면 언제든 연락해 주세요.
저희가 알지 못하면 고칠 수 없으니, 편하게 제보해 주세요. 버그인지 확실하지
않더라도 괜찮으니 이슈로 등록해 주세요.

* **Discord:** <https://discord.gg/rPWFv6W>
* **Mastodon:** <https://fosstodon.org/@wger>
* **이슈 트래커:** <https://github.com/wger-project/wger/issues>

## 소스

모든 코드와 콘텐츠는 GitHub에서 확인할 수 있습니다.

* <https://github.com/wger-project>

## 번역

[Weblate](https://hosted.weblate.org/engage/wger/)에서 앱을 여러분의 언어로
번역할 수 있습니다.

[![translation status](https://hosted.weblate.org/widgets/wger/-/multi-blue.svg)](https://hosted.weblate.org/engage/wger/)

## 라이선스

* 애플리케이션 코드: [AGPL-3.0-or-later](https://www.gnu.org/licenses/agpl-3.0.html)
* 운동/식재료 데이터: Creative Commons (개별 항목 참고)
* 문서: [CC-BY-SA-4.0](https://creativecommons.org/licenses/by-sa/4.0/)
