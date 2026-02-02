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

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

This project is configured to automatically deploy to Vercel using GitHub Actions.

### Automatic Deployment Setup

The repository includes a GitHub Actions workflow (`.github/workflows/deploy-vercel.yml`) that automatically:
- Deploys to **production** when code is pushed to the `main` branch
- Creates **preview deployments** for pull requests

### Required GitHub Secrets

To enable automatic deployments, you need to add the following secrets to your GitHub repository:

1. **`VERCEL_TOKEN`**: Your Vercel authentication token
   - Get it from: https://vercel.com/account/tokens
   
2. **`VERCEL_ORG_ID`**: Your Vercel organization ID
   - Found in your Vercel project settings or `.vercel/project.json` after running `vercel link`
   
3. **`VERCEL_PROJECT_ID`**: Your Vercel project ID
   - Found in your Vercel project settings or `.vercel/project.json` after running `vercel link`

### How to Set Up Secrets

1. Go to your GitHub repository
2. Navigate to **Settings** → **Secrets and variables** → **Actions**
3. Click **New repository secret**
4. Add each of the three secrets listed above

### Getting Vercel IDs

To get your `VERCEL_ORG_ID` and `VERCEL_PROJECT_ID`:

```bash
# Install Vercel CLI
npm install -g vercel

# Link your project
vercel link

# The IDs will be saved in .vercel/project.json
cat .vercel/project.json
```

### Manual Deployment

You can still deploy manually using the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme).

Check out the [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
