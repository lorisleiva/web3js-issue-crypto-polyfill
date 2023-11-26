Steps to reproduce:

```sh
pnpm install
node ./index.cjs
```

See error:

```
Error: This runtime does not support the generation of Ed25519 key pairs.

Install and import `@solana/webcrypto-ed25519-polyfill` before generating keys in environments that do not support Ed25519.

For a list of runtimes that currently support Ed25519 operations, visit https://github.com/WICG/webcrypto-secure-curves/issues/20
    at Object.assertKeyGenerationIsAvailable (/Users/loris/Code/web3js-test-crypto/node_modules/.pnpm/@solana+assertions@2.0.0-experimental.b036381/node_modules/@solana/assertions/dist/index.node.cjs:36:11)
    at async generateKeyPair (/Users/loris/Code/web3js-test-crypto/node_modules/.pnpm/@solana+keys@2.0.0-experimental.b036381_fastestsmallesttextencoderdecoder@1.0.22/node_modules/@solana/keys/dist/index.node.cjs:8:3)

Node.js v18.13.0
```
