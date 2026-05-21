260521_study - 社内勉強会ページ
GitHub Pagesで社内勉強会のHTMLを公開したときの備忘録。
🌐 公開URL: https://umimya3.github.io/260521_study/

📋 やったこと（手順メモ）
1. リポジトリを作成

GitHubにログイン → 右上「+」→「New repository」
Repository name を入力（例：260521_study）
「Public」 を選択（←ここ重要！Privateだと公開できない）
「Create repository」をクリック

2. index.html をアップロード

リポジトリページで「Add file」→「Upload files」
index.html をドラッグ＆ドロップ
「Commit changes」をクリック

3. imgフォルダを作成

ブラウザからはフォルダ単体を作れないのでダミーファイルで作る
「Add file」→「Create new file」
ファイル名欄に img/.gitkeep と入力（img/と打つと自動でフォルダになる！）
「Commit changes」をクリック
その後、imgフォルダ内に入って「Add file」→「Upload files」で画像をアップロード

4. GitHub Pages を有効化

リポジトリの「Settings」タブ → 左メニュー「Pages」

直接URL: https://github.com/ユーザー名/リポジトリ名/settings/pages


Branch を「main」、フォルダを「/ (root)」に設定して「Save」
数分待つと公開される 🎉


⚠️ 画像ファイル名が日本語のとき
画像ファイル名が日本語（例：勉強会資料.png）でも基本的にはGitHub Pagesで動く。
もし表示されない場合は、HTMLの <img src=""> のパスをURLエンコードに書き換える。
html<!-- 変更前 -->
<img src="img/勉強会資料.png">

<!-- 変更後（URLエンコード済み） -->
<img src="img/%E5%8B%89%E5%BC%B7%E4%BC%9A%E8%B3%87%E6%96%99.png">

URLエンコード変換ツール: https://www.urlencode.jp/


💡 知っておくと便利なこと
ファイルを直接編集できる
GitHubのブラウザ上でファイルを直接編集できる。
ファイルを開いて右上の✏️（鉛筆アイコン）をクリック → 編集 → 「Commit changes」。
変更履歴が全部残る
Commitのたびに履歴が残るので、いつ・何を変えたか追いかけられる。
リポジトリページの「X commits」をクリックで確認できる。
公開URLのパターン
https://ユーザー名.github.io/リポジトリ名/
Pages の反映には少し時間がかかる
ファイルを更新してもすぐには反映されないことがある（1〜3分ほど待つ）。
Settings → Pages に「Your site is live at ...」と表示されていればOK。
ブラウザのキャッシュに注意
更新したのに古いページが表示される場合は Ctrl + Shift + R（強制リロード）で解決することが多い。
