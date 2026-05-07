# 講義音声ノートAI

音声ファイルをアップロードするか、その場で録音すると、文字起こし・要約・要点を自動生成するWebアプリです。

## 使い方

1. アプリをブラウザで開く
2. Gemini APIキーを入力して「保存」を押す
3. 音声ファイルを選択 または「その場で録音」タブで録音
4. 「文字起こし・要約を生成」ボタンを押す
5. 文字起こし・要約・要点が表示される

## セットアップ

### APIキーの取得
1. [Google AI Studio](https://aistudio.google.com/) にアクセス
2. 「Get API key」からAPIキーを取得
3. アプリ起動時にAPIキーを入力して保存（端末内にのみ保存されます）

## 動作環境

- PC・スマホ両対応（レスポンシブ対応）
- モダンブラウザ（Chrome / Safari / Edge）

## 注意事項

- 個人情報・機密情報を含む音声はアップロードしないでください
- APIキーはGitHubリポジトリに含まれていません（localStorageに保存）

## 使用技術

- HTML / CSS / JavaScript
- Gemini API（gemini-2.0-flash）
- GitHub Pages
