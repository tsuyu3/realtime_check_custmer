# Node.js公式イメージ
FROM node:20

# 作業ディレクトリ
WORKDIR /app

# package.jsonとpackage-lock.jsonをコピー
COPY package*.json ./

# 依存関係をインストール
RUN npm install

# アプリの全ファイルをコピー
COPY . .

# React開発サーバー起動
CMD ["npm", "start"]
