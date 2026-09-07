
# 0831 - K-MOVE 동아리 MT 안내 웹앱

K-MOVE 동아리 MT(수련회) 정보를 안내하는 구글 앱스 스크립트(Google Apps Script) 기반 웹앱입니다.

## 주요 구성

- **일정표** : MT 진행 스케줄
- **준비물** : 참가자가 챙겨야 할 물품 안내
- **장소 · 집합 안내** : 집합 장소/시간, MT 장소, 이동 수단, 문의처
- **유의사항** : 참가 시 주의할 점

## 파일 구조

```
0831/
├── index.html   # MT 안내 페이지 (HTML + 인라인 CSS)
└── code.gs       # Google Apps Script 진입점 (doGet)
```

## 사용 기술

- Google Apps Script (`HtmlService`)
- HTML5 / CSS3 (인라인 스타일, 반응형 카드 UI)

## 배포 방법

`code.gs` 상단 주석에 안내된 절차를 따릅니다.

1. [script.google.com](https://script.google.com)에서 새 프로젝트 생성
2. 기본 파일에 `code.gs` 내용 붙여넣기
3. 파일 추가 > HTML > 파일명 `index`로 저장 후 `index.html` 내용 붙여넣기
4. 배포 > 새 배포 > 유형: 웹 앱 (실행 계정: 나, 액세스 권한: 모든 사용자 또는 필요에 맞게 조정)
5. 배포 후 생성된 URL로 접속
