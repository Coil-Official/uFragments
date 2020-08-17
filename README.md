# COIL


Coil (code name uFragments) is a decentralized elastic supply protocol that is inspired by Ampleforth. It maintains a stable unit price by adjusting supply directly to and from wallet holders.

The main difference between Coil and Ampleforth is supply distribution and the rebase period. Namely, Coil is a more fair and decentralized protocol with a majority of its supply being used for the initial distribution and liquidity pools. Rebase for Coil is every 23 hours and adjusts daily, having a dynamic, yet predicated rebase time.

You can read the [whitepaper](https://www.ampleforth.org/paper/) for the motivation and a complete description of the original protocol.

This repository is a collection of [smart contracts](http://ampleforth.org/docs) that implement the Coil protocol on the Ethereum blockchain.

The official mainnet addresses are:
- ERC-20 Token: [0x3936Ad01cf109a36489d93cabdA11cF062fd3d48](https://etherscan.io/token/0x3936Ad01cf109a36489d93cabdA11cF062fd3d48)
- Supply Policy: [0x7f0C14F2F72ca782Eea2835B9f63d3833B6669Ab](https://etherscan.io/address/0x7f0C14F2F72ca782Eea2835B9f63d3833B6669Ab)
- Orchestrator: [0x8A6d3D3a1b9648BbedDE7899f2B1E7410Fda2D75](https://etherscan.io/address/0x8A6d3D3a1b9648BbedDE7899f2B1E7410Fda2D75)
- Market Oracle: [0x90f98A4e55B2B07e46976e50885E1286B13aae8F](https://etherscan.io/address/0x90f98A4e55B2B07e46976e50885E1286B13aae8F)
- CPI Oracle: [0xa759f960dd59a1ad32c995ecabe802a0c35f244f](https://etherscan.io/address/0xa759f960dd59a1ad32c995ecabe802a0c35f244f)

## Table of Contents

- [Install](#install)
- [Testing](#testing)
- [Testnets](#testnets)
- [Contribute](#contribute)
- [License](#license)


## Install

```bash
# Install project dependencies
npm install

# Install ethereum local blockchain(s) and associated dependencies
npx setup-local-chains
```

## Testing

``` bash
# You can use the following command to start a local blockchain instance
npx start-chain [ganacheUnitTest|gethUnitTest]

# Run all unit tests
npm test

# Run unit tests in isolation
npx truffle --network ganacheUnitTest test test/unit/uFragments.js
```

## Contribute

To report bugs within this package, create an issue in this repository.
For security issues, please contact dev-support@ampleforth.org.
When submitting code ensure that it is free of lint errors and has 100% test coverage.

``` bash
# Lint code
npm run lint

# View code coverage
npm run coverage
```

## License

[GNU General Public License v3.0 (c) 2018 Fragments, Inc.](./LICENSE)
