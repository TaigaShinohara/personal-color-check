# コントリビュートガイド (Contributing)

バグ報告・改善提案・Pull Request を歓迎します！

## 設計方針

このプロジェクトは **「`index.html` をブラウザで開くだけで動く、ゼロビルド・完全ローカル処理の静的Webアプリ」** を基本方針としています。

- 外部サーバーへの画像送信やトラッキングスクリプトは追加しないでください
- ビルドツール（npm / webpack / Vite 等）を必須にしないでください
- 既存のプライバシー方針（写真処理は端末内のみ）を維持してください

## ローカルでの確認方法

```bash
# リポジトリをクローン
git clone https://github.com/TaigaShinohara/personal-color-check.git
cd personal-color-check

# 任意の静的サーバー、または index.html を直接ブラウザで開く
python3 -m http.server 8000
```

> カメラ機能（`getUserMedia`）をテストする場合は `http://localhost:8000` または HTTPS 経由で開いてください。

## Pull Request の手順

1. `main` から作業用ブランチを作成してください
2. 変更後、ブラウザ（PC / モバイル表示・ライト / ダークモード）でエラーが出ないことを確認してください
3. 変更内容を簡潔にまとめて Pull Request を作成してください
