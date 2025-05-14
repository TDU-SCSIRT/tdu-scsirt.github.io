# これは何?
東京電機大学の学生CSIRTのウェブサイトです。  

# このリポジトリの仕様
1. ``main``ブランチに変更が加わると自動的に本番環境にデプロイ
2. プルリクエストを作成すると、プレビュー環境にデプロイされてPRにURLがコメントされる
3. プルリクエストを作成したブランチが変更されても2が実行される

# 記事を作成するまでの手順
1. hugoをインストールする
2. このリポジトリをクローンして持ってくる

## 1. hugoのインストール
- Windows: ```winget install Hugo.Hugo.Extended```してインストール
- Mac: ```brew install hugo```してインストール
- Debian系: ```sudo apt install hugo```してインストール
- 他のLinuxディストロは各自調べてインストールしてください

## 2. リポジトリのクローン
1. Gitをインストールする
    - Windows: 初心者はGitHubデスクトップをインストール
    - Mac: 同上
    - それ以外: 調べてね
2. リポジトリをクローンする
    - 以下のでリポジトリをクローンする
    - ```git clone --recurse-submodules https://github.com/TDU-SCSIRT/tdu-scsirt.github.io.git```

# 記事の作成手順
1. クローンしたリポジトリを開く
2. 作業ディレクトリを``/scsirt``にする
3. ``hugo new content blog/[ writeup || tips ]/2025/[記事の名前].md``
4. 記事を執筆する
5. ブランチを切って、コミットとプッシュ
6. 書上げたらプルリクエストを作成し、レビューを依頼


# 担当
- @igameta: リポジトリ全体の管理とレビュー
- @BlackBeth: デザイン等のレビュー