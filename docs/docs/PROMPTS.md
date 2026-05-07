# PROMPTS.md - 使用したプロンプト

## 1. 文字起こしプロンプト
以下の音声を正確に文字起こししてください。話し言葉をそのまま書き起こしてください。
**採用理由**：シンプルに全文を書き起こすよう指示。編集不要でそのまま表示できる。

## 2. 要約・要点生成プロンプト
以下の文字起こしテキストについて、以下の2つを出力してください。
【要約】
3行程度で要約
【要点】
・箇条書きで3〜5個
文字起こし:
{transcript}
**採用理由**：【要約】【要点】のタグで出力を分けることでパースしやすくした。

## 3. 参考にした公式ドキュメント

- Gemini API モデル一覧：https://ai.google.dev/gemini-api/docs/models?hl=ja
- Gemini API 音声入力：https://ai.google.dev/gemini-api/docs/audio
- Gemini API テキスト生成：https://ai.google.dev/gemini-api/docs/text-generation
