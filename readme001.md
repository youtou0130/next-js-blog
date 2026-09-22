mkdir next-js-blog
cd next-js-blog

npx create-next-app@^15

git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/youtou0130/next-js-blog.git
git push -u origin main

git add .
git commit -m "add search"

Prisma インストール
パスワードも扱うため暗号化のbcryptjsもイン
ストール
npm install prisma@^6 @prisma/client@^6
npm install -D ts-node@^10
npm install bcryptjs@^2
npm install @types/bcryptjs@^2


npx prisma init // Prismaの初期化 
  prisma/schema.prismaと.envが生成される 
prisma/schema.prismaの設定 
provider= "sqlite" に変更 (ファイルベース 開発向けDB) 
.env ファイル 
postgresqlはコメントアウト 
DATABASE_URL="file:./dev.db" を追記


// マイグレーション(テーブル作成) 
npx prisma migrate dev --name init 
// シード実行(ダミーデータ) 
npx prisma db seed 
// DBの内容を確認 
npx prisma studio 
// DBリセット 
npx prisma migrate reset


npx shadcn@latest

npx shadcn@latest init

npm install date-fns@^4 //日付フォー
マット 
npx shadcn@latest add card


インストール方法 npm install next-auth@beta 
npm install zod@^3 
シークレットキー生成 
npx auth secret 
.env.local ファイルにAUTH_SECRETが発行される 
.envに統合


test@example.com
password123

