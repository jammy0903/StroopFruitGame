# 과일 스트룹 게임

과일 이름이 엉뚱한 배경색으로 나옴. 진짜 색깔 버튼 누르면 됨.

> "사과"가 파란 배경 → 사과는 빨간색 → **빨강** 클릭

<img src="gameplay.gif" alt="플레이 영상" width="480">

## 규칙

- 10스테이지, 스테이지당 10문제
- 7개 이상 맞추면 다음 스테이지로 넘어감
- 스테이지 올라갈수록 제한시간 짧아짐 (5초 → 1.3초)
- 정답 +10, 오답 -5, 콤보 시 추가점수
- 버튼 위치랑 배경색 매번 바뀜

## 과일

| 과일 | 색 | 해금 |
|---|---|---|
| 사과 | 빨강 | 처음부터 |
| 바나나 | 노랑 | 처음부터 |
| 블루베리 | 파랑 | 처음부터 |
| 오렌지 | 주황 | Stage 3 |
| 수박 | 초록 | Stage 5 |
| 포도 | 보라 | Stage 7 |

## 실행

**웹** — `StroopFruitGame.html` 브라우저에서 열면 됨

**APK 빌드**
```bash
export ANDROID_HOME=/path/to/android-sdk
./gradlew assembleDebug
# app/build/outputs/apk/debug/app-debug.apk
```

## 조작

- 마우스 클릭 또는 키보드 `1`~`6`
- `Space`/`Enter`로 시작/재시작

## 기술

HTML + CSS + JS 단일 파일. 외부 라이브러리 없음. 효과음은 Web Audio API로 자동 생성함. 안드로이드는 WebView로 감쌈.
