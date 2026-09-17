# 모아 — 릴리스

[모아](https://github.com/onu-soft/moa)의 **배포와 자동 업데이트**만 담는 곳입니다. 앱 소스는 비공개입니다.

## 받기

[Releases](https://github.com/onu-soft/moa-releases/releases) 에서 가장 최근 `Moa.dmg` 를 받으세요.
macOS 14 이상 · Apple Silicon 과 Intel 을 한 벌이 모두 덮습니다.

## 자동 업데이트

앱이 보는 곳은 이 저장소 `main` 의 [`latest.json`](latest.json) 하나입니다.

```
https://raw.githubusercontent.com/onu-soft/moa-releases/main/latest.json
```

`.app.tar.gz` 는 minisign 으로 서명되어 있고, 앱에 박힌 공개키와 맞아야만 설치됩니다.
서명이 안 맞으면 업데이트는 조용히 거부됩니다.

> 🚨 `latest.json` 은 **릴리스 자산이자 `main` 의 파일**입니다. 자산만 올리면
> 아무도 업데이트를 받지 못합니다 — 앱 저장소의 `pnpm upload:publish` 가 둘 다 합니다.
