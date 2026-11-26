# ROADMAP（上から順に。週1の自動更新で1つずつ進める）

各項目の（）内は、Googleの検索候補（suggestqueries.google.com、2026-11-26取得）で実際に出た語。記事のタイトルと見出しにその語を入れる。

1. Gemini の料金を追加（2026-12-01 の価格改定後に公式ページで確認してから）
2. ガイド：Claude Codeの使用量・料金の確認方法（「claude code 料金確認」「claude code プラン確認」「claude code プラン 確認 コマンド」）… /usage 等。公式ドキュメントのみを根拠に
3. ガイド：Claude Codeの設定ファイルの場所と一覧（「claude code 設定ファイル 場所」「claude code 設定ファイル 一覧」「claude code 設定 おすすめ」）… settings.json のスコープ
4. ガイド：プロンプトキャッシュとは・Claudeでの料金（「プロンプトキャッシュとは」「プロンプトキャッシュ claude」「プロンプトキャッシュ 時間」）… 5分・1時間、書き込み割増を含めた計算例
5. ガイド：Claude APIの無料枠と始め方（「claude api 料金 無料 枠」「claude api キー 使い方」）… 公式に無料枠の記載がなければ「ない」と書かず、確認できた事実だけ
6. 計算機：キャッシュ書き込み（5分1.25倍・1時間2倍）を任意で入れられるようにする
7. CLAUDE.md作成ツール：`.claude/rules/` の paths 付きルールファイルも作れるようにする

## 完了
- ガイド：Claude APIとClaude Codeの料金の違い（2026-11-26）
- ガイド：CLAUDE.mdとAGENTS.md・スキル・rulesの違い（「claude.md agents.md」「claude.md skills 違い」、2026-11-26）
- ガイド末尾に筆者のnote記事へのリンク（tools/note_links.py、deploy.sh で毎回更新）

## 守ること
- 料金・仕様は必ず公式ページで確認し、出典URLと確認日を載せる。確認できないものは載せない
- 新しい記事の題材は、Googleの検索候補で実際に出る語から選ぶ（取得コマンドは 自動更新手順.md）
- 公開前に `node tests/check.mjs` がすべてOK、公開後に `node tests/live.cjs` で本番確認
