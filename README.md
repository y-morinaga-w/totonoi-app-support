# Totonoi App - GitHub Pages

このディレクトリには、App Store Connectで必要なサポートページとプライバシーポリシーページが含まれています。

## セットアップ手順

### 1. GitHubリポジトリの作成

1. GitHubにログインし、新しいリポジトリを作成します
   - リポジトリ名: `totonoi-support`（任意の名前でOK）
   - 公開設定: Public（GitHub PagesはPublicリポジトリで無料）
   - READMEは追加しなくてOK

### 2. ファイルのアップロード

このディレクトリ内の以下のファイルをGitHubリポジトリにアップロードします：

- `index.html` - サポートページ
- `privacy.html` - プライバシーポリシーページ

**アップロード方法：**

#### 方法A: GitHub Web UI
1. リポジトリのページで「Add file」→「Upload files」をクリック
2. `index.html`と`privacy.html`をドラッグ&ドロップ
3. 「Commit changes」をクリック

#### 方法B: Gitコマンド
```bash
cd github-pages
git init
git add index.html privacy.html
git commit -m "Initial commit: Add support and privacy pages"
git branch -M main
git remote add origin https://github.com/[your-username]/totonoi-support.git
git push -u origin main
```

### 3. GitHub Pagesの有効化

1. リポジトリの「Settings」タブを開く
2. 左メニューから「Pages」を選択
3. 「Source」で「Deploy from a branch」を選択
4. 「Branch」で「main」（または「master」）を選択
5. 「/ (root)」を選択
6. 「Save」をクリック

### 4. URLの確認

数分待つと、以下のURLでアクセスできるようになります：

```
https://[your-username].github.io/totonoi-support/
https://[your-username].github.io/totonoi-support/privacy.html
```

例：
- `https://yukiwatanabe.github.io/totonoi-support/`
- `https://yukiwatanabe.github.io/totonoi-support/privacy.html`

### 5. App Store Connectへの登録

1. App Store Connectにログイン
2. アプリ情報 > 日本語 を選択
3. 以下のURLを入力：
   - **サポートURL**: `https://[your-username].github.io/totonoi-support/`
   - **プライバシーポリシーURL**: `https://[your-username].github.io/totonoi-support/privacy.html`

## カスタマイズ

### メールアドレスの変更

`index.html`の以下の部分を編集してください：

```html
<p class="email">📧 support@totonoi.app</p>
```

### プライバシーポリシーの更新

`privacy.html`の内容を、アプリの実際のデータ収集・利用方法に合わせて編集してください。

### デザインの変更

両ファイルの`<style>`タブ内のCSSを編集することで、デザインをカスタマイズできます。

## 注意事項

- GitHub Pagesは無料で利用できますが、Publicリポジトリである必要があります
- リポジトリ名を変更すると、URLも変更されます
- ファイルを更新した後、反映まで数分かかる場合があります
- カスタムドメインを使用する場合は、GitHub Pagesの設定でドメインを追加できます

