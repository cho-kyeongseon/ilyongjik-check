# HANDOFF

## 지금까지 한 작업
- 2026-11-08: 일용직 판정 도구 첫 버전(index.html) 작성, GitHub·Vercel 배포.
- 2026-11-12: USB 폴더와 GitHub 저장소(main) 연결 상태 확인 — 내용 동일.
  Vercel Git 연동 확인(main 푸시마다 자동 배포). .gitignore, CLAUDE.md, HANDOFF.md 추가.

## 현재 상태
- index.html 한 파일로 동작하며 배포 중: https://ilyongjik-check.vercel.app
- 알려진 오류 없음. 이번 세션에서 index.html 코드는 바꾸지 않았음.

## 남은 일
- 정해진 다음 작업 없음. 새 요청이 생기면 여기에 적는다.

## 주의할 점
- 원본 엑셀(고객 자료)은 커밋하지 않는다(.gitignore에서 *.xlsx, *.xls, *.xlsm, *.csv 제외).
- USB(exFAT)라 다른 PC나 다른 드라이브 문자에서 git이 "dubious ownership" 오류를 내면:
  `git config --global --add safe.directory '<드라이브>:/주말수업/일용직'`
- 엑셀 읽기 라이브러리(SheetJS 0.18.5)를 cdnjs에서 불러오므로 인터넷 연결이 필요하다.

## 실행 방법
- 설치할 것 없음. index.html을 브라우저로 열거나 배포 주소에 접속한다.
- 엑셀(원천2_일용직 / 고객개요 시트)을 화면에 끌어다 놓으면 판정 결과가 나온다.
- 배포: main에 푸시하면 Vercel이 자동 배포한다.

## 원본 자료 위치
- 원본 엑셀은 GitHub에 없고 USB(또는 각자 PC)에만 둔다.
- 프로그램은 고정 경로를 읽지 않는다. 사용자가 브라우저에서 파일을 끌어다 놓거나 선택한 파일만 읽고,
  처리는 브라우저 안에서만 한다(서버 전송 없음).
