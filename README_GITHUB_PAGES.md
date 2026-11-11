# デジタル工事黒板カメラ GitHub Pages版

## 公開ファイル

同じリポジトリのルートへ、次の3ファイルを配置してください。

- `index.html`
- `manifest.webmanifest`
- `sw.js`

## GitHub Pagesで公開する手順

1. GitHubで新しいリポジトリを作成します。
2. 上記3ファイルをリポジトリ直下へアップロードし、`Commit changes`を実行します。
3. リポジトリの `Settings` → `Pages` を開きます。
4. `Build and deployment` の `Source` を `Deploy from a branch` にします。
5. `Branch` を `main`、フォルダーを `/(root)` にして `Save` を押します。
6. 公開完了後に表示される `https://ユーザー名.github.io/リポジトリ名/` をiPhoneのSafariで開きます。
7. Safariの共有ボタン → `ホーム画面に追加` を選択します。

## iPhoneでの初回確認

- カメラ使用の確認が表示されたら `許可` を選択してください。
- GitHub PagesはHTTPS配信のため、ブラウザのカメラAPIを使用できます。
- 初回表示後はService Workerが基本ファイルをキャッシュします。
- 更新が反映されない場合は、Safariのタブを閉じて再度開くか、ホーム画面のアイコンを削除して追加し直してください。

## 注意事項

- リポジトリをPublicにすると、HTMLとJavaScriptのソースは第三者から閲覧できます。
- 工事名、会社名、撮影内容などの入力値はブラウザの`localStorage`へ保存されます。
- 撮影画像はサーバーへ自動送信せず、端末内で合成・保存します。
- GitHub Pagesのプロジェクトサイトでも動くように、URLはすべて相対パスで設定しています。
