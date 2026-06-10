# 일본어 단어장 PWA - GitHub Pages 배포 가이드

## 파일 목록
- `index.html` - 메인 앱
- `manifest.json` - PWA 설정
- `sw.js` - 오프라인 지원
- `words_n1.js` ~ `words_n5.js` - N1~N5 단어 데이터
- `icon-192.png`, `icon-512.png` - 앱 아이콘

---

## GitHub Pages 배포 방법 (5분)

### 1단계: GitHub에서 새 저장소 만들기
1. https://github.com 로그인
2. 우측 상단 **+** 버튼 → **New repository**
3. Repository name: `jlpt-flashcard` (원하는 이름)
4. **Public** 선택
5. **Create repository** 클릭

### 2단계: 파일 업로드
1. 저장소 페이지에서 **uploading an existing file** 클릭
2. 위의 모든 파일을 한꺼번에 드래그 앤 드롭
3. **Commit changes** 클릭

### 3단계: GitHub Pages 활성화
1. 저장소 → **Settings** 탭
2. 왼쪽 메뉴 **Pages** 클릭
3. Source: **Deploy from a branch**
4. Branch: **main** / **/ (root)**
5. **Save** 클릭

### 4단계: 접속 (약 1~2분 후)
```
https://[GitHub계정명].github.io/jlpt-flashcard/
```

---

## 아이폰 홈 화면에 추가 (앱처럼 사용)
1. 아이폰 Safari에서 위 주소 접속
2. 하단 공유 버튼(□↑) 탭
3. **홈 화면에 추가** 탭
4. 이름 확인 후 **추가** 탭
5. 홈 화면에 앱 아이콘이 생성됩니다!

---

## 기능
- N1~N5 단어 2,498개 (예문 포함)
- 스테이지 분할 학습 (10/20/30/50/100개)
- 외움 / 못 외움 / 북마크 기능
- 좌우 스와이프로 외움 판정
- 일본어 TTS 발음 듣기
- 학습 통계
- 오프라인 지원 (PWA)
- 진행 상황 자동 저장 (브라우저 로컬 스토리지)
- 한국어/일본어 UI 전환
