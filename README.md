# mimermoeをdockerで簡単に立てる
1. リポジトリをクローン
```
git clone https://github.com/nr1a/misskey-docker/
cd misskey-docker
```
2. 設定ファイル（中身を見ながら自分で調整してください）
```
cp .config/docker_example.yml .config/default.yml
cp .config/docker_example.env .config/docker.env
cp ./docker-compose_example.yml ./docker-compose.yml
```
3. 初期化
```
sudo docker compose run --rm web pnpm run init
```
4. 起動
```
sudo docker compose up -d
```
