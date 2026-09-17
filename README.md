# 統一地方選挙2027 特設サイト

第21回統一地方選挙（2027年）向けの静的特設ページです。  
HTML・CSS・JavaScript・画像・選挙区データのみで動作します。

## 構成

```
.
├── index.html                      # 特設ページ本体
├── senkyo2027/
│   ├── election-districts-data.js  # 選挙区データ
│   └── img/                        # 画像・SVG
├── serve.py                        # ローカルプレビュー用
└── README.md
```

## ローカルで確認

```bash
python3 serve.py
```

ブラウザで http://127.0.0.1:8080/ を開いてください。

## GitHub へアップロード

このフォルダをそのまま新規リポジトリのルートに置けます。

```bash
cd senkyo2027-github   # このフォルダ
git init
git add .
git commit -m "Add 2027 unified local election special site"
git branch -M main
git remote add origin git@github.com:YOUR_ORG/YOUR_REPO.git
git push -u origin main
```

## GitHub Pages

1. リポジトリの Settings → Pages
2. Source: Deploy from a branch
3. Branch: `main` / `/ (root)`
4. 公開 URL の `/` が `index.html` になります

## 補足

- ヘッダー・フッターは後日共通コンポーネントへ差し替え予定のスタブです
- 選挙区データは `senkyo2027/election-districts-data.js` に同梱しています
- 投票マッチング・My選挙・外部リンクは go2senkyo.com 等の本番 URL です
