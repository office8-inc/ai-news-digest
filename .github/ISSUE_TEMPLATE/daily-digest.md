---
name: 📰 Daily Digest Request
about: AI News Daily Digest の自動収集リクエスト
labels: copilot
---

# 🤖 AI News Daily Digest

## 収集対象日
YYYY-MM-DD

## 収集対象サイト
1. **MIT Technology Review** - https://www.technologyreview.com/topic/artificial-intelligence/
2. **VentureBeat AI** - https://venturebeat.com/category/ai/
3. **TechCrunch AI** - https://techcrunch.com/tag/artificial-intelligence/
4. **The Verge AI** - https://www.theverge.com/ai-artificial-intelligence
5. **Towards Data Science** - https://towardsdatascience.com/
6. **Wired (AI)** - https://www.wired.com/tag/artificial-intelligence/

## 出力形式
- 各サイトから1-2件の重要記事を選定
- 日本語で要約を作成
- 記事タイトル・見出し・参考リンクのリンクテキストも日本語で記述する
- 10分で読める分量（約2000-3000文字）
- 実践的なアクションアイテムを含める

## 重複防止
- `.article-history/articles-history.json` の履歴を確認
- 過去7日分の記事との重複をチェック
- 重複記事は自動的にスキップ
- 収集後、Copilotが履歴ファイルを自動更新

## 出力先
`daily/YYYY-MM-DD.md`

---

@copilot 上記の収集対象サイトから最新のAI関連ニュースを収集し、要約を作成してください。
