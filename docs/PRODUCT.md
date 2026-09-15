# V1 Trench Radar: product brief

## Job to be done

Define filters for new meme launches that use atomic v1 creation patterns.

## User flow

1. Connect a Wallet Standard wallet to identify the creator and inspect v1 support.
2. Edit the supplied trend example.
3. Generate a deterministic `txv1-labs/1` artifact with a SHA-256 content digest.
4. Inspect encoded bytes, predicted v1 parts, and transaction savings over legacy.
5. Copy or download the artifact for review and later publication.

## Architecture

The site is dependency-free HTML, CSS, and browser JavaScript. All transforms and hashes run locally with Web Crypto. The production build copies an immutable static artifact to `dist/`; Wrangler serves that directory from Cloudflare Workers. No secret, RPC key, wallet key, or user content crosses a project-owned server.

## Production boundary

This release is safe to deploy as a non-custodial generator. It does not claim that an estimate will always fit after a wallet modifies a transaction, and it does not broadcast. A production signing release must use `@solana/kit >= 8`, simulate explicit resource limits, verify the selected wallet advertises v1, and add end-to-end tests against Solana CLI 4.2+ before enabling mainnet.

## Growth loop

Every downloaded artifact includes the product slug and a deterministic content hash. A future verified gallery can index successful transactions, reassemble multipart records, and issue a share card without central custody.
