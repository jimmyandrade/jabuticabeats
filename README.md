This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Dependency Management

This project uses npm (Node Package Manager) and relies on the `package-lock.json` file to ensure that all developers and build environments use the exact same versions of project dependencies. This practice is crucial for maintaining consistency and avoiding "works on my machine" issues.

**Recommended Installation Command:**

For most cases, especially in CI/CD pipelines or when setting up the project for the first time, it is recommended to use:

```bash
npm ci
```

This command installs dependencies strictly based on `package-lock.json`, which can be faster and more reliable than `npm install` for ensuring reproducible builds. `npm install` should be used when you intend to update your dependencies or add new ones (which will, in turn, update `package-lock.json` if needed).

**Other Package Managers:**

While `npm` and `package-lock.json` are the primary mechanisms for this project, if you prefer using Yarn, pnpm, or Bun (as mentioned in the "Getting Started" section), these tools also generate and use their own lock files (`yarn.lock`, `pnpm-lock.yaml`, and `bun.lockb`, respectively) to achieve the same goal of pinned, reproducible dependency installations.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
