
# 0901 - 자취/독립생활 실태 설문조사

편의점 영수증 콘셉트의 디자인으로 제작한 자취(독립생활) 실태 설문조사 웹앱입니다. Google Apps Script로 배포하며, 응답 결과는 Google 스프레드시트에 자동 저장됩니다.

## 주요 구성

- **설문 항목**
  - 독립기간 (`period`)
  - 거주형태 (`residence`)
  - 월생활비 (`livingCost`)
  - 주거비 부담도 (`burden`)
  - 자취 애로사항 (`difficulties`, 다중 선택)
  - 만족도 (`satisfaction`)
- **제출 완료 화면** : 설문 제출 후 안내 페이지 표시

## 동작 방식

1. `doGet()` 이 `index.html`을 웹페이지로 렌더링합니다.
2. 사용자가 폼을 작성하고 제출하면 클라이언트가 `google.script.run`으로 `submitForm(data)`를 호출합니다.
3. `submitForm`은 필수 항목(독립기간, 거주형태)을 검증한 뒤 지정된 Google 스프레드시트(`SHEET_URL`)에 응답을 한 행씩 추가합니다.

## 파일 구조

```
0901/
├── index.html   # 설문 폼 페이지 (영수증 디자인)
└── Code.gs       # Google Apps Script (doGet, submitForm)
```

## 사용 기술

- Google Apps Script (`HtmlService`, `SpreadsheetApp`)
- HTML5 / CSS3 / JavaScript

## 배포 방법

1. `Code.gs`의 `SHEET_URL`을 실제 사용할 구글 스프레드시트 주소로 교체
2. 스프레드시트 첫 번째 탭 1행에 다음 순서로 헤더 작성: `독립기간 | 거주형태 | 월생활비 | 주거비부담도 | 자취애로사항 | 만족도`
3. Apps Script 프로젝트에 `Code.gs`, `index.html` 등록 후 웹 앱으로 배포
