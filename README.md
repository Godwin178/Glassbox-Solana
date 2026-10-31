# Glassbox-Solana

Glassbox-Solana is a read-only Solana transparency and accountability toolkit built with TypeScript and Solana Web3.js.

This repository contains a working MVP for:

- Public wallet inspection
- Transaction signature verification and exploration
- Funding and expense transparency
- Project milestone tracking
- Public transparency reports
- Community proposals and voting overview
- A responsive dashboard

## Security and compliance

All blockchain inspection is read-only. The project never requests or stores private keys or seed phrases.

## Requirements

- Node.js 20+
- npm
- A Solana RPC endpoint

## Environment setup

Create a `.env.local` file in the project root with a read-only Solana RPC URL:

```bash
SOLANA_RPC_URL=https://api.mainnet-beta.solana.com
```

You may also use a devnet or custom RPC endpoint if preferred.

## Run locally

```bash
npm install
npm run dev
```

Then open http://localhost:3000

## Tests

```bash
npm test
```

## Production build

```bash
npm run build
npm run start
```

## GitHub permissions and 403 errors

A 403 Forbidden error from a GitHub integration usually indicates one of the following:

1. The GitHub App or bot does not have repository access.
2. The repository is protected by branch rules and the integration cannot push.
3. The integration is not granted write access to the repo.
4. The app is authenticated to the wrong GitHub account or organization.
5. The integration lacks the required permissions for contents, workflows, or pull requests.

The fix is to check:

- Repository → Settings → Collaborators and teams
- Repository → Settings → Actions → General
- Repository → Settings → Branches
- GitHub App authorization for the integration

Do not share private keys, access tokens, or passwords. The application never needs them for read-only blockchain inspection.

## Features implemented

- Read-only public wallet inspection
- Signature search and transaction detail view
- Funding transparency dashboard with sample public records
- Milestone tracker and community proposal data
- Downloadable transparency report generation
- Mobile-friendly dashboard

## License

MIT
