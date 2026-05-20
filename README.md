# 静岡心不全連携システム（しずおかハートリンク）

## 📋 プロジェクト概要

静岡市における心不全患者の地域連携システムのウェブサイトです。
かかりつけ医・専門医・多職種が連携し、早期介入からACP・看取りまで
シームレスなケアを提供するための情報共有プラットフォームです。

## 📂 ファイル構成

```
shizuoka-heart-link/
├── index.html              # メインページ
├── sheet-A.html            # 連携シートA（かかりつけ医→専門医）
├── sheet-B.html            # 連携シートB（専門医→かかりつけ医）
├── images/                 # 画像ファイル
│   ├── flow-diagram.jpg    # 連携フロー図
│   └── reimbursement-diagram.jpg  # 診療報酬改定図
├── downloads/              # ダウンロード資料
│   ├── sheet-A.xlsx        # 連携シートA（Excel版）
│   └── sheet-B.xlsx        # 連携シートB（Excel版）
└── README.md               # このファイル
```

## 🎨 デザイン仕様

- **カラー**: 静岡医師会ブルー（#1e4d7b）
- **背景**: 純白（#ffffff）
- **BNP 5段階分類**: 医療的な落ち着いた配色
- **レスポンシブ対応**: PC・タブレット・スマートフォン

## 🌐 GitHub Pagesへのデプロイ方法

### ステップ1: GitHubリポジトリの作成

1. GitHubにログイン（https://github.com）
2. 右上の「+」→「New repository」をクリック
3. リポジトリ名を入力（例: `shizuoka-heart-link`）
4. 「Public」を選択
5. 「Create repository」をクリック

### ステップ2: ファイルのアップロード

**方法A: ブラウザから直接アップロード（簡単！）**

1. 作成したリポジトリページで「uploading an existing file」をクリック
2. このフォルダ内の**全てのファイルとフォルダ**をドラッグ&ドロップ
   - ⚠️ 重要: フォルダ構造をそのまま維持してアップロード
3. 下の「Commit changes」をクリック

**方法B: Git コマンドを使用（上級者向け）**

```bash
# このフォルダに移動
cd shizuoka-heart-link

# Gitの初期化
git init

# 全ファイルを追加
git add .

# コミット
git commit -m "Initial commit: 静岡心不全連携システム"

# GitHubリポジトリと接続（URLは自分のリポジトリに変更）
git remote add origin https://github.com/ユーザー名/shizuoka-heart-link.git

# アップロード
git branch -M main
git push -u origin main
```

### ステップ3: GitHub Pagesの有効化

1. GitHubのリポジトリページで「Settings」タブをクリック
2. 左メニューから「Pages」を選択
3. 「Source」のドロップダウンで「main」ブランチを選択
4. フォルダは「/ (root)」を選択
5. 「Save」をクリック

### ステップ4: 公開URLの確認

約1〜2分後、同じPages設定画面に
**「Your site is live at https://ユーザー名.github.io/shizuoka-heart-link/」**
と表示されます。このURLが公開URLです！

## ✅ 動作確認

デプロイ後、以下を確認してください：

- [ ] メインページ（index.html）が正しく表示される
- [ ] フロー図の画像が表示される
- [ ] 連携シートA・Bのリンクが動作する
- [ ] Excelファイルのダウンロードが可能
- [ ] スマートフォンでも正しく表示される

## 🔧 トラブルシューティング

### 画像が表示されない
→ `images/` フォルダがリポジトリにアップロードされているか確認

### ダウンロードファイルが動作しない
→ `downloads/` フォルダがリポジトリにアップロードされているか確認

### ページが404エラー
→ GitHub Pagesの設定で「main」ブランチが選択されているか確認

### スマホで表示が崩れる
→ ブラウザのキャッシュをクリアしてから再読み込み

## 🔄 ファイルを更新する方法

ファイルを更新する場合：

1. GitHubのリポジトリページで該当ファイルをクリック
2. 鉛筆アイコン（Edit）をクリック
3. 内容を編集
4. 「Commit changes」をクリック
5. 約1分後、自動的にサイトが更新されます

## 📞 お問い合わせ

静岡市静岡医師会
- ウェブサイト: https://shizuoka-city-shizuoka-med.jp
- メール: info@shizuoka-city-shizuoka-med.jp

---

© 2026 静岡市静岡医師会・静岡市清水医師会
