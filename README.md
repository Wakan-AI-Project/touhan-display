# 登録販売者勤務状況 — 会社管理用の並行公開

会社管理先：Wakan-AI-Project/touhan-display

既存の公開ページ https://imuimu9631.github.io/touhan-display/ を残したまま、会社側で表示・取得を確認するためのコピーです。公式HPのリンクや旧URLの転送は変更していません。

- 元ソース：imuimu9631/touhan-display、commit 2e2f8d163f58197accfb777efde44cdcbe61f7b0
- 入口：site/index.html（元ファイルと同一）
- 勤務情報：既存Google Apps Scriptを使用。GAS・勤務表の所有権や設定は変更していません。
- 公開：GitHub Pages / Actions。手動実行のみ。対象会社repoと明示入力を確認してsite/のみ配備。

日付別のブラウザキャッシュを使い、当日分がない場合に勤務情報を取得します。同日の途中変更や開きっぱなしでの日付切替を即時反映する仕組みではありません。

site/staff-schedule.htmlは原本に含まれる補助ファイルで、PHP include・共通部品への依存があります。GitHub PagesでPHP実行されるものではなく、この補助ページの完全動作は保証しません。通常の入口index.htmlを確認対象とします。

新URLからの取得・日付・不在日・取得失敗時の表示とキャッシュを確認した後、公式HPや旧URLの切替は別途判断します。
