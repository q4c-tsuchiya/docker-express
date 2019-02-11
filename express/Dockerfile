# ベースイメージを指定
FROM node:10.12

# 環境変数設定
ENV NODE_ENV="development"

# 作業ディレクトリ作成&設定
ENV APP_ROOT /src

COPY mysrc/package.json $APP_ROOT
RUN npm install && npm cache clean

COPY . $APP_ROOT
EXPOSE 3000
CMD ["npm", "start"]


