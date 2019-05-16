# 概要
nuxtをgaeでホスティングする

# 手順
```
// nuxtアプリ作成
vue init nuxt-community/starter-template nuxt-app

// ローカルで表示確認
cd nuxt-app
npm install
npm run dev

// ビルド
// nuxt-app/nuxt.config.js を変更してビルド先を backend/dist に変更しておく
npm run generate

// gaeサーバー起動
cd ../backend
dev_appserver.py app.yaml
```