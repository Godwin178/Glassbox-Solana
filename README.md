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
