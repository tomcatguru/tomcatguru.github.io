# 톰리의 개발 노트

[공개 블로그](https://tomcatguru.github.io/)의 Jekyll 소스입니다. GitHub Pages가 `master` 브랜치의 루트에서 빌드합니다.

## 글 추가하기

`_posts/YYYY-MM-DD-글-주소.md` 파일을 만들고 제목, 날짜, 요약, 태그를 적습니다. 본문은 Markdown으로 이어서 작성합니다.

```yaml
---
title: 글 제목
description: 글의 한 줄 요약
date: 2026-11-18 09:00:00 +0900
tags: [모바일, 오디오]
---
```

홈의 최신 글 목록, 아카이브, 태그 페이지, RSS는 글에서 자동으로 만들어집니다. 대표 작업은 `_data/work.yml`, 소개는 `about.md`에서 편집합니다.

## 로컬에서 보기

Ruby 3.3과 Bundler가 있는 환경에서 다음 명령을 실행합니다.

```sh
bundle install
bundle exec jekyll serve
```

브라우저에서 `http://localhost:4000`을 엽니다.
