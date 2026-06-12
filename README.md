# 일본어 단어장 PWA

Flutter 윈도우 앱을 PWA로 변환한 버전입니다.

## 파일 목록 (10개)
- `index.html` — 메인 앱 (HTML + CSS + JS 통합)
- `manifest.json` — PWA 설정
- `sw.js` — 오프라인 지원 (네트워크 우선 전략)
- `words_n1.js` ~ `words_n5.js` — N1~N5 단어 데이터 (2,498개)
- `icon-192.png`, `icon-512.png` — 앱 아이콘

## GitHub Pages 배포

1. GitHub 저장소의 기존 파일 전부 삭제
2. 위 10개 파일을 드래그 앤 드롭 업로드
3. Settings → Pages → main / root → Save
4. `https://shunkanmono.github.io/jlpt_flashcard/` 접속

## Flutter → PWA 대응표

| Flutter 파일 | PWA 대응 |
|---|---|
| `study_provider.dart` | `index.html` JS state (S 객체) |
| `flashcard_widget.dart` | `renderCard()`, `onCardTap()` |
| `flashcard_screen.dart` | 다이얼로그, 레벨바 |
| `settings_panel.dart` | `renderSettingsPanel()` |
| `stats_panel.dart` | `renderStatsPanel()` |
| `progress_bar_widget.dart` | `renderProgressBar()` |
| `control_bar_widget.dart` | #controlbar HTML |
| `ruby_text_widget.dart` | `parseRuby()` |
| `word.dart` | JS word 객체 구조 |
| `jlpt_words.dart` | `words_n1~n5.js` |
