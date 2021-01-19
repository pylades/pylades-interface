# Pylades Interface 💂

[![Lint](https://github.com/pylades/pylades-interface/workflows/Lint/badge.svg)](https://github.com/pylades/pylades-interface/actions?query=workflow%3ALint)
[![Tests](https://github.com/pylades/pylades-interface/workflows/Tests/badge.svg)](https://github.com/pylades/pylades-interface/actions?query=workflow%3ATests)
[![Styled With Prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://prettier.io/)

An open source interface for Pylades -- a protocol for decentralized exchange of Ethereum tokens.

- Website: [pylades.finance](https://pylades.finance/)
- Interface: [app.pylades.finance](https://app.pylades.finance)
- Docs: [pylades.finance/docs/](https://docs.pylades.finance)
- Twitter: [@PyladesProtocol](https://twitter.com/PyladesProtocol)
- Reddit: [/r/pylades](https://www.reddit.com/r/PyladesProtocol/)
- Email: [contact@pylades.finance](mailto:contact@pylades.finance)
- Discord: [pylades](https://discord.gg/Y7TF6QA)
- Whitepaper: [Link](https://hackmd.io/C-DvwDSfSxuh-Gd4WKE_ig)

## Accessing the Pylades Interface

To access the Pylades Interface, use an IPFS gateway link from the
[latest release](https://github.com/pylades/pylades-interface/releases/latest),
or visit [app.pylades.finance](https://app.pylades.finance).

## Listing a token

Please see the
[@pylades/default-token-list](https://github.com/pylades/default-token-list)
repository.

## Development

### Install Dependencies

```bash
yarn
```

### Run

```bash
yarn start
```

### Configuring the environment (optional)

To have the interface default to a different network when a wallet is not connected:

1. Make a copy of `.env` named `.env.local`
2. Change `REACT_APP_NETWORK_ID` to `"{YOUR_NETWORK_ID}"`
3. Change `REACT_APP_NETWORK_URL` to e.g. `"https://{YOUR_NETWORK_ID}.infura.io/v3/{YOUR_INFURA_KEY}"`

Note that the interface only works on testnets where both
[Pylades V2](https://pylades.finance/docs/v2/smart-contracts/factory/) and
[multicall](https://github.com/makerdao/multicall) are deployed.
The interface will not work on other networks.

## Contributions

**Please open all pull requests against the `master` branch.**
CI checks will run against all PRs.

## Accessing Pylades Interface V1

The Pylades Interface supports swapping against, and migrating or removing liquidity from Pylades V1. However,
if you would like to use Pylades V1, the Pylades V1 interface for mainnet and testnets is accessible via IPFS gateways
linked from the [v1.0.0 release](https://github.com/pylades/pylades-interface/releases/tag/v1.0.0).
