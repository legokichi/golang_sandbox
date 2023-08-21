# project layout



- https://github.com/golang-standards/project-layout/blob/master/README_ja.md


## makefile
 https://zenn.dev/rosylilly/articles/202105-go-makefile

- ./          # リポジトリルート。 package gochat
- bin/        # バイナリを吐く場所。gitignore する。
- cmd/        # バイナリのパッケージ
  - server/   # サーバーバイナリ。 package main
    - main.go # エントリーポイント
  - client/   # クライアントバイナリ。 package main
    - main.go # エントリーポイント
- proto/      # .proto ファイル置き場
- .gitignore  # gitignore ファイル
- go.mod      # go.mod
- go.sum      # go.sum
- Makefile    # 肝心要の奴
- gochat.go   # バージョン情報なんかを埋める対象
