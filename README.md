# gemini-ask

Gemini APIを使用したシンプルなCLIツール。

## インストール

**GitHubから直接実行（推奨）:**

```bash
uvx git+https://github.com/okunarutakashi/gemini-ask "質問内容"
```

**ローカルインストール:**

```bash
uvx --from /path/to/gemini-ask gemini_ask "質問内容"
# または
uv run gemini_ask "質問内容"
```

## 使用方法

```bash
# 基本的な使用方法
gemini_ask "今日の天気は？"

# モデルを指定
gemini_ask "量子力学について教えて" --model "gemini-2.5-pro"
```

## 環境変数

以下のいずれかの環境変数を設定してください：

- `GEMINI_API_KEY` (優先)
- `GOOGLE_API_KEY`

`.env`ファイルを使用することもできます。

## 依存関係

- Python >= 3.10
- google-genai >= 1.63.0
- python-dotenv >= 1.2.1
