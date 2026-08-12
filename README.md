# ML Workshop Portal

별도 빌드 없이 브라우저에서 바로 확인할 수 있는 단일 페이지 워크숍 포털입니다.

## 로컬에서 확인하기

저장소 루트에서 아래 명령을 실행하세요.

```bash
python3 -m http.server 8000
```

그런 다음 브라우저에서 <http://localhost:8000>을 열고 입장 코드
`ml-workshop-2026`을 입력합니다.

> `index.html` 파일을 직접 열어도 되지만, 브라우저 보안 정책에 따른 동작 차이를
> 피하려면 로컬 HTTP 서버 사용을 권장합니다.

## 확인할 화면

- **홈**: 수다타임, 보드게임, 워크숍 안내 진입 카드
- **안내**: 일정, 장소, 근태, 조 편성, 케이터링, 회식 메뉴 및 예산
- **수다타임**: 중복 없이 뽑히는 24개의 랜덤 대화 카드
- **보드게임**: 게임별 소개와 규칙 모달

## GitHub Pages 배포

`work` 브랜치에 변경 사항을 푸시하면 GitHub Actions가 정적 사이트를 GitHub
Pages에 자동으로 배포합니다. 저장소의 **Settings → Pages → Build and
deployment → Source**가 **GitHub Actions**로 설정되어 있어야 합니다.

필요한 경우 Actions 화면의 **Deploy to GitHub Pages** 워크플로에서
**Run workflow**를 눌러 수동으로 다시 배포할 수도 있습니다.
