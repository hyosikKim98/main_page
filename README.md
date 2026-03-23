# GitHub Pages 포트폴리오

이 폴더에는 GitHub Pages에 바로 올릴 수 있는 정적 포트폴리오 페이지가 들어 있습니다.

## 로컬 확인

브라우저에서 `index.html`을 직접 열어도 되고, 아래처럼 간단한 정적 서버로 확인해도 됩니다.

```bash
python3 -m http.server 8000
```

그 다음 브라우저에서 `http://localhost:8000`에 접속하면 됩니다.

## GitHub Pages 배포

1. 이 폴더 내용을 GitHub 저장소 루트에 올립니다.
2. `index.html`이 저장소 루트에 있는지 확인합니다. GitHub Pages는 `index.html`, `index.md`, `README.md` 중 하나를 엔트리 파일로 찾습니다.
3. 저장소에서 `Settings > Pages`로 이동합니다.
4. `Build and deployment`에서 `Deploy from a branch`를 선택합니다.
5. 배포 브랜치를 `main`과 `/ (root)`로 지정한 뒤 저장합니다.
6. 반영까지 몇 분 걸릴 수 있으며, 보통 GitHub Pages 주소가 생성되면 바로 접속할 수 있습니다.

`.nojekyll` 파일도 함께 넣어 두었기 때문에, Jekyll 처리 없이 현재 정적 파일을 그대로 배포할 수 있습니다.

## 수정 포인트

- 메인 소개 문구와 프로젝트 내용은 `index.html`에서 바로 수정할 수 있습니다.
- 색상과 레이아웃은 `styles.css`의 `:root` 변수와 각 섹션 클래스를 수정하면 됩니다.
- GitHub, 블로그, 연락처 링크를 추가하려면 `index.html`의 상단 버튼 영역과 문서 섹션의 링크를 교체하면 됩니다.
