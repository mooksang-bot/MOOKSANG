# 작업 규칙 (사용자 요청으로 저장)

## 웹을 고칠 때마다 보고하는 방법
- 웹(claude.ai 아티팩트)을 고치거나 게시하면, 끝 보고에 **PC 웹**과 **휴대폰 웹** 링크를 두 줄로 따로 적는다.
  - 형식: `PC 웹` 링크 한 줄, `휴대폰 웹 (아이폰·삼성폰)` 링크 한 줄. 누를 수 있는 링크로 적는다.
- 고친 뒤에는 오른쪽 화면에 결과를 띄운다.
  - Artifact 도구의 `open`으로 고친 웹을 연다.
  - 고친 화면을 PC 크기(1280×800)와 휴대폰 크기(390×844)로 찍어서 오른쪽 화면에 보여 준다. SendUserFile을 쓰고 display는 render로 한다.
- 사용자의 컴퓨터가 연결된 세션이라 내장 브라우저(오른쪽 창)를 직접 다룰 수 있으면, 사용자가 고른 링크(PC 또는 휴대폰)를 그 크기로 오른쪽 창에 띄운다.
  - PC는 desktop 크기, 휴대폰은 mobile 크기로 띄운다.

## 웹 목록
- 엘리사 수학 교실: https://claude.ai/artifact/Uy3a4EgyVVn9ffyqfLgPW6 (`elisa-math.html`, 기록: `ELISA_MATH.md`)
- 제자 훈련 [기초반]: https://claude.ai/artifact/NPJuoiZmYBS64ck3DDiE44 (`discipleship.html`, 기록: `DISCIPLESHIP.md`)

## 이어서 작업하기
- 사용자가 "엘리사 수학 웹 불러오기"라고 하면:
  1. `ELISA_MATH.md`의 "지금 상태"를 먼저 읽는다.
  2. `elisa-math.html`을 그 상태에서부터 이어서 고친다. 새로 만들지 않는다.
  3. 게시는 같은 주소(위 웹 목록)로 한다.
- "제자 훈련 웹 불러오기"도 같은 방식으로 한다. `DISCIPLESHIP.md`와 `discipleship.html`을 쓴다.

## 그 밖의 선호
- 쉬운 한국어로 설명한다.
- 사용자가 "실행"이라고 하면 확인 질문 없이 바로 진행한다.
- 작업이 끝나면 PushNotification으로 휴대폰 알림(진동)을 보낸다. 무엇이 끝났는지 한 줄로 적는다.
