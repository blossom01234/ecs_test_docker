# ベースイメージの指定
FROM node:18

# 作業ディレクトリを設定
WORKDIR /app

# Gitをインストールしてリポジトリからコードを取得
RUN apt-get update && apt-get install -y git

# Gitリポジトリからアプリケーションコードを取得
RUN git clone https://github.com/blossom01234/ecs_test_backend.git .

# 依存関係のインストール
RUN npm install

# アプリケーションポートを公開
EXPOSE 3000

# アプリケーションの起動コマンド
CMD ["npm", "start"]
