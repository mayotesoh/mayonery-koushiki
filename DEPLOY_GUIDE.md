# 手相のマヨネリ - GitHub Pages デプロイガイド

## 📦 必要なファイル構成

```
手相のマヨネリ/
├── index.html          ✅ トップページ
├── kouza.html          ✅ 手相講座ページ
├── kantei.html         ✅ 手相鑑定ページ
├── gakkai.html         ✅ 手相学会ページ
├── shindan.html        ✅ 手相診断ページ
├── css/
│   └── style.css       ✅ スタイルシート
├── js/
│   └── main.js         ✅ JavaScript
├── images/
│   ├── wariai.png      ⚠️ 追加が必要
│   ├── kihonkantei.png ⚠️ 追加が必要
│   ├── zikidasi.png    ⚠️ 追加が必要
│   └── kanteisyo.png   ⚠️ 追加が必要
└── README.md           ✅ プロジェクト説明
```

## 🖼️ 画像ファイルの準備

### ステップ1: AIドライブから画像をダウンロード

AIドライブの `/マヨネリ公式サイト/` フォルダから、以下の4つの画像をダウンロードしてください：

1. **wariai.png** - 受講者の割合の円グラフ
2. **kihonkantei.png** - 基本鑑定の画像
3. **zikidasi.png** - 流年鑑定の画像
4. **kanteisyo.png** - 鑑定書の画像

### ステップ2: imagesフォルダに配置

ダウンロードした4つの画像を `images/` フォルダに配置してください。

## 🚀 GitHub Pages へのデプロイ手順

### 1. GitHubリポジトリの作成

1. GitHub (https://github.com) にログイン
2. 右上の「+」→「New repository」をクリック
3. リポジトリ名を入力（例: `mayotesoh-official-site`）
4. 「Public」を選択
5. 「Create repository」をクリック

### 2. ファイルのアップロード

#### 方法A: GitHub Web UI を使用（簡単）

1. 作成したリポジトリのページで「uploading an existing file」をクリック
2. すべてのファイルとフォルダをドラッグ&ドロップ
3. 「Commit changes」をクリック

#### 方法B: Git コマンドを使用

```bash
# ローカルでリポジトリを初期化
cd 手相のマヨネリ
git init
git add .
git commit -m "Initial commit: 手相のマヨネリ公式サイト"

# GitHubにプッシュ
git branch -M main
git remote add origin https://github.com/mayotesoh/[リポジトリ名].git
git push -u origin main
```

### 3. GitHub Pages の設定

1. リポジトリのページで「Settings」をクリック
2. 左サイドバーの「Pages」をクリック
3. 「Source」で「Deploy from a branch」を選択
4. 「Branch」で「main」ブランチを選択
5. フォルダは「/ (root)」を選択
6. 「Save」をクリック

### 4. サイトの公開確認

数分後、以下のURLでサイトが公開されます：
```
https://mayotesoh.github.io/[リポジトリ名]/
```

## ✅ チェックリスト

デプロイ前に以下を確認してください：

- [ ] すべてのHTMLファイルが配置されている
- [ ] css/style.css が配置されている
- [ ] js/main.js が配置されている
- [ ] images/ フォルダに4つの画像が配置されている
- [ ] 画像ファイル名が正しい（wariai.png, kihonkantei.png, zikidasi.png, kanteisyo.png）

## 🔧 トラブルシューティング

### 画像が表示されない場合

1. 画像ファイル名が正確に一致しているか確認
2. 画像が `images/` フォルダに配置されているか確認
3. ファイル名の大文字・小文字が一致しているか確認

### ページが表示されない場合

1. GitHub Pages の設定が正しいか確認
2. index.html がルートディレクトリにあるか確認
3. 数分待ってからリロード

## 📝 カスタマイズ

デプロイ後のカスタマイズ方法は README.md をご参照ください。

---

## 🎉 完成！

上記の手順を完了すれば、手相のマヨネリの公式Webサイトが GitHub Pages で公開されます！

何か問題がございましたら、GitHubのIssuesでご質問ください。