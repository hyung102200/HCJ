날짜별 폴더로 구성된 개인 웹 프로젝트 모음입니다. 각 폴더는 독립적인 프로젝트이며, 대부분 별도의 빌드 과정 없이 `index.html`을 브라우저에서 열거나 로컬 웹 서버로 바로 확인할 수 있습니다.

## 프로젝트 목록

### [0723](0723/) - 권우형 포트폴리오 페이지
경성대학교 컴퓨터공학과 재학생 권우형의 개인 포트폴리오 웹페이지. 터미널/코드 에디터 느낌의 다크 테마 디자인에 스크롤 진행률 표시, 타이핑 애니메이션 효과를 적용했으며, TravelBusan·타닥(Tadak) 등의 프로젝트 이력을 소개합니다.
- 기술: HTML5 / CSS3 / Vanilla JavaScript, Google Fonts
- 실행: `index.html`을 브라우저에서 열기

### [0724](0724/) - 권우형의 이력서 (기본 버전)
HTML/CSS로 제작한 초기 형태의 개인 이력서 페이지. 프로필, 자기소개, 연락처, 기술 스택, 프로젝트(캡스톤 DB 연동 영상 등)를 소개합니다.
- 기술: HTML5 / CSS3 (별도 JavaScript 없음)
- 실행: `index.html`을 브라우저에서 열기

### [0727](0727/) - 권우형의 이력서 (다국어/테마 지원 버전)
0724 버전을 발전시킨 이력서 페이지로, 반응형 2단 레이아웃과 한국어/영어/일본어 다국어 전환, 다크·라이트 테마 전환 기능이 추가되었습니다.
- 기술: HTML5 / CSS3 (반응형), Vanilla JavaScript (다국어 전환, 테마 토글, 타이핑 효과)
- 실행: `index.html`을 브라우저에서 열기

### [0831](0831/) - K-MOVE 동아리 MT 안내 웹앱
K-MOVE 동아리 MT(수련회) 일정, 준비물, 장소·집합 안내, 유의사항을 안내하는 Google Apps Script 기반 웹앱입니다.
- 기술: Google Apps Script (`HtmlService`), HTML5 / CSS3
- 실행: script.google.com에 배포 후 웹 앱 URL로 접속 (`code.gs` 상단 주석 참고)

### [0901](0901/) - 자취/독립생활 실태 설문조사
편의점 영수증 콘셉트로 디자인한 설문조사 웹앱. 응답 결과는 Google 스프레드시트에 자동 저장됩니다.
- 기술: Google Apps Script (`HtmlService`, `SpreadsheetApp`), HTML5 / CSS3 / JavaScript
- 실행: `Code.gs`의 `SHEET_URL`을 교체 후 Apps Script 프로젝트로 배포

### [0907](0907/) - KOREA JOURNEY | 일본인 대상 한국 관광 안내 웹사이트
일본인 관광객을 대상으로 서울·부산·제주도 명소, K-FOOD, 여행 준비 정보(WOWPASS, eSIM, 관광통역 등)를 소개하는 반응형 관광 포털 웹사이트입니다.
- 기술: HTML5, Tailwind CSS(CDN), jQuery 3.7.1 / Vanilla JavaScript
- 실행: `index.html`을 브라우저에서 직접 열거나 로컬 웹 서버(`python3 -m http.server`)로 실행
