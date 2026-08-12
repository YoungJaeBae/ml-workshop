# 2026 상반기 회고

별도 빌드 없이 브라우저에서 바로 작성할 수 있는 A4 한 장짜리 상반기 회고지입니다.

## 로컬에서 확인하기

저장소 루트에서 아래 명령을 실행하세요.

```bash
python3 -m http.server 8000
```

그런 다음 브라우저에서 <http://localhost:8000>을 엽니다.

> `index.html` 파일을 직접 열어도 되지만, 브라우저 보안 정책에 따른 동작 차이를
> 피하려면 로컬 HTTP 서버 사용을 권장합니다.

## 주요 기능

- 이름과 10개의 회고 답변을 화면에서 바로 작성
- 상반기 날씨와 만족도 선택
- A4 인쇄 및 PDF 저장
- 작성한 회고지를 PNG 이미지로 저장
- 작성 내용 전체 초기화

## GitHub Pages 배포

`work` 브랜치에 변경 사항을 푸시하면 GitHub Actions가 정적 사이트를 GitHub
Pages에 자동으로 배포합니다. 저장소의 **Settings → Pages → Build and
deployment → Source**가 **GitHub Actions**로 설정되어 있어야 합니다.

필요한 경우 Actions 화면의 **Deploy to GitHub Pages** 워크플로에서
**Run workflow**를 눌러 수동으로 다시 배포할 수도 있습니다.
