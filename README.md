# 方極 주치 조합 검색 — 웹앱 설치 안내

## 들어 있는 파일
- index.html : 프로그램 본체
- manifest.webmanifest : 앱 이름, 아이콘, 색상 정보
- sw.js : 오프라인 실행을 위한 파일
- icons/ : 앱 아이콘

네 가지를 **폴더 구조 그대로** 한 곳에 올려야 합니다.

## GitHub Pages에 올리기 (무료)
1. github.com 에서 무료 계정을 만듭니다.
2. 오른쪽 위 + → New repository. 이름을 예: `fangji` 로 정하고, Public 선택 후 Create.
3. 새 저장소 화면에서 "uploading an existing file" 링크를 누르고,
   압축을 푼 폴더 안의 파일과 icons 폴더를 통째로 끌어다 놓은 뒤 Commit changes.
4. 저장소의 Settings → Pages 로 가서
   Source: Deploy from a branch / Branch: main, / (root) → Save.
5. 1~2분 뒤 `https://아이디.github.io/fangji/` 주소가 생깁니다. 이 링크를 공유하면 됩니다.

## 휴대폰·PC에 설치하기
- 안드로이드(크롬): 주소를 열면 화면 위 "앱으로 설치" 버튼이 나타납니다. 없으면 메뉴 ⋮ → 홈 화면에 추가.
- 아이폰(사파리): 공유 버튼 → 홈 화면에 추가.
- PC(크롬·엣지): 주소창 오른쪽의 설치 아이콘, 또는 화면 위 "앱으로 설치".

처음 한 번 인터넷에 연결된 상태로 열어 두면, 이후에는 오프라인에서도 한자 글꼴까지 그대로 작동합니다.

## 내용을 고쳤을 때
1. 수정한 index.html 을 GitHub 저장소에 다시 올립니다 (Add file → Upload files, 같은 이름으로 덮어쓰기).
2. sw.js 첫 줄의 `fangji-v1` 을 `fangji-v2` 처럼 숫자를 올려 함께 올립니다.
3. 사용자는 앱을 한두 번 다시 열면 새 버전으로 바뀝니다.
