# 우리 애 우주

반려동물의 여러 모습(자세)을 사진으로 찍어 배경을 지우고, 아이만의 행성 위에 차곡차곡 쌓아 기록하는 아카이브 앱이에요.

## 구성
- `www/` — 앱 화면 (HTML·CSS·JS 한 파일 + 물리 엔진 `matter.min.js`)
- `android/` — Capacitor 안드로이드 프로젝트
- `.github/workflows/build-apk.yml` — `main`에 푸시하면 APK를 빌드해 **Releases → 최신 빌드**에 올려요

## APK 받기
GitHub 저장소의 **Releases → 최신 빌드**에서 `pet-universe.apk`를 내려받아 설치하세요.
처음 설치할 때 "출처를 알 수 없는 앱 설치 허용"이 필요해요.

## 로컬에서 빌드하기
```bash
npm ci
npx cap sync android
cd android && ./gradlew assembleDebug
```
결과물: `android/app/build/outputs/apk/debug/app-debug.apk`
