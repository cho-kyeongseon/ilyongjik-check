# CLAUDE.md

일용직 판정 도구 — 엑셀을 브라우저에서 읽어 일용직 여부와 소득세를 계산하는 HTML 한 파일(index.html). 자세한 설명은 README.md.

## 작업 규칙
- 작업 폴더는 USB이고, GitHub는 백업과 Vercel 배포용이다.
- 기본 작업 브랜치는 main. 다른 브랜치는 요청할 때만 쓴다.
- 작업이 한 단락 끝나면 HANDOFF.md를 업데이트한다.

## 참고
- GitHub: https://github.com/cho-kyeongseon/ilyongjik-check (main)
- Vercel: https://ilyongjik-check.vercel.app — main에 푸시하면 자동 배포된다.
- 원본 엑셀 등 고객 자료는 .gitignore로 제외되어 있다. 커밋하지 않는다.
- 프로그램은 파일을 브라우저 업로드(드래그&드롭)로 읽으므로 드라이브 문자에 의존하는 경로가 없다. 새 코드에서도 절대 경로(E:\ 등)를 쓰지 않는다.
- USB(exFAT)라서 다른 PC나 다른 드라이브 문자에서 git이 "dubious ownership" 오류를 내면 그 경로를 `git config --global --add safe.directory '<경로>'`로 추가한다.
