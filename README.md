# Prisma-ORM

# 1️⃣ Create a new project folder and navigate into it
mkdir my-prisma-project && cd my-prisma-project

# 2️⃣ Initialize a Node.js project
npm init -y

# 3️⃣ Install Prisma and PostgreSQL client
npm install @prisma/client @prisma/cli pg

# 4️⃣ Initialize Prisma
npx prisma init

# 5️⃣ Configure PostgreSQL connection in .env
# Edit the .env file and set:
# DATABASE_URL="postgresql://USER:PASSWORD@HOST:PORT/DATABASE?schema=public"

# 6️⃣ Define schema in prisma/schema.prisma
# Edit schema.prisma and define models

# 7️⃣ Generate Prisma Client
npx prisma generate

# 8️⃣ Run initial migration
npx prisma migrate dev --name init

# 9️⃣ Push schema changes (if needed)
npx prisma db push

# 🔟 Check database tables
npx prisma studio

# 1️⃣1️⃣ Seed the database (if applicable)
npx prisma db seed

# 1️⃣2️⃣ Use Prisma in TypeScript
# Create a new file (e.g., index.ts) and add:
# import { PrismaClient } from "@prisma/client";
# const prisma = new PrismaClient();

# 1️⃣3️⃣ Run TypeScript code
npx ts-node index.ts

# 1️⃣4️⃣ Disconnect Prisma after usage
# await prisma.$disconnect();
