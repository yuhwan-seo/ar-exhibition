# Web AR 전시관 (GitHub Pages용)

이 폴더는 GitHub Pages에 바로 올릴 수 있게 정리된 정적 사이트입니다.

## 파일 구성
- `index.html` : 전시관 메인 파일
- `.nojekyll` : GitHub Pages의 Jekyll 처리 비활성화

## 배포 방법 (가장 쉬운 방식)
1. GitHub에서 새 저장소를 만듭니다.
2. 이 폴더 안의 파일들을 저장소 루트에 업로드합니다.
3. 저장소의 **Settings → Pages** 로 이동합니다.
4. **Build and deployment** 에서 **Source = Deploy from a branch** 를 선택합니다.
5. **Branch = main**, **Folder = /(root)** 를 선택하고 저장합니다.
6. 잠시 뒤 배포 주소가 생성됩니다.

예시 주소:
- `https://사용자이름.github.io/저장소이름/`

## 실행 팁
- 모바일 브라우저에서 여세요.
- 카메라 권한을 허용하세요.
- `Hiro` 마커를 비추면 AR 전시관이 나타납니다.

## 수정 포인트
- 작품 설명: `index.html`의 `const artworks` 객체
- 전시관 제목: 상단 HUD 텍스트
- 작품 패널 이미지: `<a-assets>` 내부의 SVG gradient 이미지
- 3D 오브젝트: 중앙 `a-sphere`, `a-torus-knot` 또는 GLB 모델로 교체 가능

## 주의
- GitHub Pages는 정적 파일 호스팅입니다.
- 일부 모바일 브라우저/권한 설정에서는 카메라 접근 허용이 필요합니다.
