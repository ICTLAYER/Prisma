# Nuxt 3 + Prisma + MySQL 8

Look at the [Nuxt 3 + Prisma documentation](https://www.prisma.io/docs/reference/api-reference/command-reference) to learn more.

## Setup

Make sure to install the dependencies:

```bash
# Nuxt 3
npm install

# Prisma
npm install prisma --save-dev
npx prisma init
npm install typescript ts-node @types/node --save-dev
npx prisma generate
npm install @prisma/client
npx prisma db pull
```

Change .env db_name

## Browse your data

Start server on `http://localhost:5555`:

```bash
# Browse your data
npx prisma studio
```

## Production

Build the application for production:

```bash
# npm
npm run build

# pnpm
pnpm run build

# yarn
yarn build
```

Locally preview production build:

```bash
# npm
npm run preview

# pnpm
pnpm run preview

# yarn
yarn preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.
