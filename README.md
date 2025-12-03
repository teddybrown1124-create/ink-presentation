# LINK公式説明資料 - Vercel/Netlifyデプロイガイド

## 🌐 プロジェクト概要

これはLINK公式説明資料(60ページ)を誰でもアクセスできるWebサイトとして公開するためのデプロイガイドです。

**特徴**
- ✅ **60ページの完全なプレゼンテーション**
- ✅ **深いブルー × ゴールド**のモダンデザイン
- ✅ **30枚以上の実写真**:link-event-x.comからの実際のLINKイベント写真
- ✅ **データ視覚化**:ビッグナンバー、3Dピラミッド、グラフ
- ✅ **超大型写真版**:写真が主役のインパクトのあるデザイン

----

## 📋 必要な前提条件

デプロイを始める前に、以下のアカウントを準備してください:

1. **GitHubアカウント**:[GitHub.com](https://github.com)で無料アカウントを作成
2. **VercelまたはNetlifyアカウント**:どちらか一方を選択
   - [Vercel.com](https://vercel.com) (推奨)
   - [Netlify.com](https://netlify.com)
3. **基本的なWebブラウザ操作の知識**

**注意**:すべて無料プランで始められます!

----

## 🚀 デプロイ方法

以下の3つの方法から選択できます:

### 方法1:Vercelでデプロイ(推奨)

#### ステップ1:GitHubリポジトリを作成

1. **[GitHub.com](https://github.com)にログイン**
2. 右上の**「+」→「New repository」**をクリック
3. リポジトリ設定:
   - リポジトリ名:`link-presentation`(例)
   - **Public**を選択(誰でもアクセス可能)
   - 「Add a README file」にチェック(推奨)
4. **「Create repository」**をクリック

#### ステップ2:HTMLファイルをアップロード

1. リポジトリページで**「Add file」→「Upload files」**をクリック
2. **`index.html`をドラッグ&ドロップ**
3. コミットメッセージを入力(例:「Add LINK presentation landing page」)
4. **「Commit changes」**をクリック

#### ステップ3:Vercelでデプロイ

1. **[Vercel.com](https://vercel.com)にアクセス**
2. **GitHubアカウントでサインアップ**
3. **「Add New」→「Project」**をクリック
4. **GitHubリポジトリを選択**:`link-presentation`
5. **「Deploy」**をクリック
6. **数分待つ**:ビルドが完了するまで待機
7. **公開URLが生成されます!**
   - 例:`https://link-presentation.vercel.app`

----

### 方法2:Netlifyでデプロイ

#### ステップ1:GitHubリポジトリを作成

(方法1と同じ手順)

#### ステップ2:HTMLファイルをアップロード

(方法1と同じ手順)

#### ステップ3:Netlifyでデプロイ

1. **[Netlify.com](https://netlify.com)にアクセス**
2. **GitHubアカウントでサインアップ**
3. **「Add new site」→「Import an existing project」**をクリック
4. **GitHubリポジトリを選択**:`link-presentation`
5. **「Deploy site」**をクリック
6. **数分待つ**:ビルドが完了するまで待機
7. **公開URLが生成されます!**
   - 例:`https://link-presentation.netlify.app`

----

### 方法3:GitHub Pagesでデプロイ(無料)

#### ステップ1:GitHubリポジトリを作成

(方法1と同じ手順)

#### ステップ2:HTMLファイルをアップロード

(方法1と同じ手順)

#### ステップ3:GitHub Pagesを有効化

1. リポジトリページで**「Settings」**をクリック
2. 左サイドバーで**「Pages」**をクリック
3. **「Source」**で**「main」ブランチ**を選択
4. **「Save」**をクリック
5. **数分待つ**:デプロイが完了するまで待機
6. **公開URLが生成されます!**
   - 例:`https://YOUR_USERNAME.github.io/link-presentation/`

----

## 🌐 カスタムドメイン設定

独自ドメイン(例:`link-presentation.com`)を設定したい場合:

### Vercelの場合

1. Vercelプロジェクトページで**「Settings」→「Domains」**をクリック
2. **独自ドメインを入力**(例:`link-presentation.com`)
3. **DNS設定を行う**:Vercelが指示するCNAMEレコードをドメインレジストラに追加
4. **数時間待つ**:DNSの伝播に時間がかかります

### Netlifyの場合

1. Netlifyサイト設定で**「Domain settings」**をクリック
2. **「Add custom domain」**をクリック
3. **独自ドメインを入力**
4. **DNS設定を行う**:Netlifyが指示するCNAMEレコードを追加

----

## 🔧 トラブルシューティング

### 問題1:デプロイが失敗する

**解決策**:
- `index.html`がリポジトリのルートディレクトリにあることを確認
- HTMLファイルに文法エラーがないか確認
- ビルドログを確認し、エラーメッセージを確認

### 問題2:ページが404エラーになる

**解決策**:
- `index.html`が正しくアップロードされているか確認
- GitHub Pagesの場合:デプロイに10分程度かかることがあります
- ブラウザのキャッシュをクリアしてみる

### 問題3:デザインが崩れる

**解決策**:
- `index.html`に必要なCSS/JavaScriptファイルが含まれているか確認
- フォントやアイコンのCDNリンクが正しいか確認
- 画像URLが正しくアクセスできるか確認

### 問題4:カスタムドメインが機能しない

**解決策**:
- DNS設定が正しいか確認
- DNSの伝播に24時間程度かかることがあります
- DNS設定ツール(例:https://www.whatsmydns.net/)で伝播状況を確認

----

## ❓ FAQ

### Q1:無料で公開できますか?

**A:**はい!Vercel、Netlify、GitHub Pagesすべて無料プランで利用できます。

### Q2:どの方法がおすすめですか?

**A:****Vercel**を推奨します。理由:
- デプロイが高速(数分)
- 自動SSL証明書
- CDN経由で世界中どこからでも高速アクセス
- カスタムドメイン設定が簡単

### Q3:プレゼンテーションを更新したい場合は?

**A:**
1. GitHubリポジトリで`index.html`を更新
2. コミット&プッシュ
3. Vercel/Netlifyが自動で再デプロイします!

### Q4:モバイルでも見られますか?

**A:**はい!`index.html`はレスポンシブ対応なので、PC、タブレット、スマホで快適に見られます。

### Q5:PPTXファイルも一緒に公開できますか?

**A:**はい!PPTXファイルもGitHubリポジトリにアップロードし、`index.html`からダウンロードリンクを追加できます。

----

## 📞 サポート

問題が解決しない場合は、以下のリソースを参照してください:

- **Vercelドキュメント**:[https://vercel.com/docs](https://vercel.com/docs)
- **Netlifyドキュメント**:[https://docs.netlify.com](https://docs.netlify.com)
- **GitHub Pagesドキュメント**:[https://docs.github.com/pages](https://docs.github.com/pages)

----

## 📅 更新履歴

- **2025-12-03**:初版リリース

----

© 2025 LINK Co., Ltd. All rights reserved.
