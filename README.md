# Prisma-ORM

```
mkdir my-prisma-project && cd my-prisma-project
npm init -y
npm install @prisma/client @prisma/cli pg ts-node typescript @types/node --save-dev
npx prisma init
npx prisma generate
npx prisma migrate dev --name init
npx prisma db push
npx prisma studio
npx prisma db seed
npx ts-node index.ts

```
