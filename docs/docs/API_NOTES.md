# API_NOTES.md - API情報

## 使用API

- **Gemini API**（Google）
- 公式ドキュメント：https://ai.google.dev/gemini-api/docs

## 使用モデル

- `gemini-2.0-flash`
- 音声入力・テキスト生成両対応
- 最新モデル一覧：https://ai.google.dev/gemini-api/docs/models?hl=ja

## エンドポイント
https://generativelanguage.googleapis.com/v1beta/models/gemini-2.0-flash:generateContent
## リクエスト形式

### 音声（文字起こし）
```json
{
  "contents": [{
    "parts": [
      { "inline_data": { "mime_type": "audio/webm", "data": "BASE64" } },
      { "text": "文字起こしのプロンプト" }
    ]
  }]
}
```

### テキスト（要約）
```json
{
  "contents": [{
    "parts": [
      { "text": "要約のプロンプト" }
    ]
  }]
}
```

## 制限・注意事項

- APIキーはlocalStorageに保存（GitHubリポジトリには含めない）
- 音声は短いもの（30秒〜2分）で検証推奨
- 対応音声形式：audio/webm, audio/mp4, audio/m4a, audio/wav, audio/mp3

## APIキーの取得方法

1. https://aistudio.google.com/ にアクセス
2. 「Get API key」をクリック
3. 新しいAPIキーを作成
