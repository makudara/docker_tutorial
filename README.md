# docker_tutorial
docker で開発環境を作るあれこれ

# docker 環境の設定

1. 動かしたい環境を決める
  + python
  + vue.js+fastAPI 
2. dockerのインストール
3. docker imageのpull
4. dockerコンテナを起動
5. docker image をbuildする
6. python を実行する

# よくある質問

+ Q: dockerってなに？
  + A: docker とは
  + 大雑把にいうとPC内に仮想的な環境を構築するアプリケーション
+ Q: VMとの違いは？
  + A: docker VM 違い
  + VMはPCそのものを仮想的に作って、Dockerは必要なパーツだけを構築するイメージ
  + Dockerの方が細かい制御ができる分、複雑
+ Q: どうやって使うの？
  + A: docker インストール mac
  + 大まかに言うと、インストール→イメージ作成→コンテナ起動 の手順
+ Q: イメージ？
  + A: docker イメージ
  + 実体化する前の仮想環境。class的な存在をイメージして貰えば大体OK
  + これを引っ張ってきたり(pull) 作ったり(build)して準備する
  + たい焼き機の型
+ Q: コンテナ？
  + A: docker コンテナ
  + 実際に操作できるイメージの具体化。メモリとか資源が割り当てられてる状態
  + classと同じで、同じイメージだけど違うコンテナとかも作れる
  + たい焼き機で作ったたい焼きそのもの
+ Q: イメージの作り方は？
  + A: docker image python
  + 誰かが作ってくれたのを引っ張ってくる方法。基本的にはこれで済ませたい。
  + https://hub.docker.com
  + A: docker image build
  + 自分でイメージを作る方法。実際には細かい調整が必要なので、こっちになることが多い
  + Dockerfileと呼ばれる設計図を作って、それをbuildすることでイメージを作成する
+ Q: Dockerfileの作り方
  + A: dockerfile python
  + ベースのimageを決める→必要なコマンドを並べる
  + イメージとしては新しい環境で色々インストールする操作を書き込むシェルスクリプトを作る感じ
+ Q: コンテナの起動のしかた
+ Q: コンテナの使い方
+ Q: コンテナの終了の仕方
