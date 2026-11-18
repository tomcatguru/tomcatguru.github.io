# Engineering Garden 글 작성 및 발행 안내

GitHub 저장소의 `master` 브랜치에 있는 `_posts` 폴더에 영문 Markdown 파일을 추가하면 발행됩니다. **A Checklist for Audio SDK Changes**를 예시로 따라 해 보세요.

## 1. 글 파일 만들기

저장소의 `master` 브랜치 루트에서 **Add file → Create new file**을 선택하고, 파일 이름 칸에 아래 경로를 입력하세요. [Engineering Garden 저장소](https://github.com/tomcatguru/tomcatguru.github.io/tree/master)

```text
_posts/2026-11-18-a-checklist-for-audio-sdk-changes.md
```

편집기에 아래 내용을 붙여 넣으세요. 두 `---` 사이에는 제목, 요약, 발행일, 태그를 적고, 그 아래부터 Markdown으로 본문을 씁니다.

```markdown
---
title: "A Checklist for Audio SDK Changes"
description: "Three quick checks for a mobile app after an audio SDK change."
date: 2026-11-18 09:00:00 +0900
tags:
  - iOS
  - Audio SDKs
---

Before I update an audio SDK, I write down what the app should do during a normal recording and when something interrupts it.

## Three checks

1. Record a short clip, stop, and play it back.
2. Interrupt a recording and check that the app makes its status clear.
3. Switch from the built-in microphone to a headset and verify which input the app uses.

For each check, I note the device, OS version, and what happened. That gives me a baseline for the next SDK update.
```

실제 글을 쓸 때는 **파일명 앞의 날짜와 `date`의 날짜를 맞추세요.** 서울 시간은 `+0900`으로 표시합니다. 바로 발행하려면 현재 시각이나 그 이전을 적으세요. `description`은 Notes와 Writing 목록에 표시할 영문 한 줄 요약입니다.

## 2. 태그 달기

`tags:` 아래에 **태그 하나당 `-` 한 줄**을 씁니다. 위 예시에서 `iOS`와 `Audio SDKs`는 각각 하나의 태그입니다. 발행하면 글 상단과 Tags 페이지에 자동으로 표시됩니다. [Tags 페이지](https://tomcatguru.github.io/tags/)

같은 주제로 계속 쓸 때는 **같은 이름과 대소문자**를 재사용하세요. `iOS`와 `ios`는 별도 태그로 묶입니다. 이 예시처럼 플랫폼(`iOS`)과 주제(`Audio SDKs`)를 하나씩 고르면 관련 글을 찾기 쉽습니다.

## 3. 발행하고 확인하기

1. 편집기의 **Preview** 탭에서 제목과 목록 형식을 확인하세요.
2. **Commit changes…**를 누르고 커밋 메시지에 `Add audio SDK checklist`를 입력하세요. **Commit directly to the master branch**를 선택한 뒤 커밋하면 GitHub Pages가 자동으로 배포를 시작합니다. [GitHub Pages 글 발행 안내](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-content-to-your-github-pages-site-using-jekyll)
3. Actions에서 **pages build and deployment**가 성공하면 블로그 홈의 **Notes**를 확인하세요. 최신 5편은 Notes에, 전체 글은 Writing에 표시됩니다. [Actions](https://github.com/tomcatguru/tomcatguru.github.io/actions) · [Notes](https://tomcatguru.github.io/#notes) · [Writing](https://tomcatguru.github.io/archive/)

이 예시를 발행하면 글 주소는 `/2026/11/18/a-checklist-for-audio-sdk-changes/`가 됩니다.
