mkdir next-js-blog
cd next-js-blog

npx create-next-app@^15

git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/youtou0130/next-js-blog.git
git push -u origin main


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



