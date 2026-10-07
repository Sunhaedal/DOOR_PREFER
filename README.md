# 게임 기획 과제 포트폴리오

게임 기획 과제를 모은 정적 포트폴리오 사이트입니다. GitHub에 올리면 Vercel이 자동으로 배포합니다.

## 구성

| 파트 | 내용 |
|---|---|
| 미메시스 이벤트 기획서 | 협동 공포 게임 미메시스의 할로윈 시즌 한정 이벤트 기획 |
| 트릭컬 재미요소 과제 | 트릭컬 리바이브의 재미요소를 직접 찾은 것과 조사한 것으로 나눠 분류 |

## 폴더 구조

```
DOOR_PREFER/
├─ index.html              # 포트폴리오 본문 (파트별 section)
├─ css/
│  └─ style.css            # 전체 스타일
├─ assets/
│  └─ img/
│     └─ mimesis-keyart.png
├─ 미메시스_할로윈_이벤트_기획서.md   # 기획서 원문
├─ vercel.json
├─ .gitignore
└─ README.md
```

## 새 파트 추가하기

1. `index.html`의 `<main>` 안에 `<section class="part" id="새이름">`을 추가합니다.
2. 상단 `topnav`와 `project-links`에 링크를 한 줄씩 추가합니다.
3. 이미지는 `assets/img/`에 넣고 `<img src="assets/img/파일명">`으로 불러옵니다.

## 배포

별도 빌드가 필요 없는 정적 사이트입니다.

1. `git add . && git commit -m "내용" && git push`
2. Vercel에서 이 저장소를 Import합니다. Framework Preset은 `Other`, Build Command와 Output Directory는 비워 둡니다.
3. 이후에는 push할 때마다 자동으로 다시 배포됩니다.
