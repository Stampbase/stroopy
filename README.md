# Stroopy

> The stroopy.me application — the Stroopy character protocol and reference renderer.

Part of [Stroop](https://github.com/Stampbase), an open identity layer for
Stellar, built by [Stampbase](https://github.com/Stampbase).

## Where this fits

Stroopy is the visual character layer. Character ownership and traits are
distinct from Stroop profile identity: a profile may have no Stroopy, and
owning a Stroopy is independently verifiable rather than implied by a profile.
Identity itself lives in [`stroop-contracts`](https://github.com/Stampbase/stroop-contracts).

## Status

**Pre-alpha.** Scaffolding only. No renderer, asset pack, or character
protocol has been implemented yet.

Nothing here is deployed to Stellar mainnet. Do not use any part of this
repository to custody value.

### Planned scope

- Deterministic SVG character renderer with a versioned renderer identifier
- Asset manifest format with content hashes and layer ordering
- Permanent numbered character pages (`stroopy.me/6261`)
- Username to active Stroopy resolution (`stroopy.me/bastian`)
- Ownership presentation, distinct from any claim of NFT ownership

## Running it

```bash
npm install
cp .env.example .env.local
npm run dev
```

## Testing

```bash
npm run lint
npx tsc --noEmit
npm run build
```

## Security

Do not report vulnerabilities through public issues. See
[`SECURITY.md`](./SECURITY.md) for private reporting.

## License

[Apache-2.0](./LICENSE).

## Related repositories

| Repository | Purpose |
| --- | --- |
| [`stroop-contracts`](https://github.com/Stampbase/stroop-contracts) | Soroban contracts: identity registry, usernames, wallet links |
| [`stroop-sdk`](https://github.com/Stampbase/stroop-sdk) | `@stroop-id/sdk` and `@stroop-id/react` |
| [`stroop-web`](https://github.com/Stampbase/stroop-web) | stroop.id — identity application |
| [`stroopy`](https://github.com/Stampbase/stroopy) | stroopy.me — character application |
| [`stroop-docs`](https://github.com/Stampbase/stroop-docs) | Protocol specifications |
