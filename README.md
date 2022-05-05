# nft-demo

## Summary

This is a demo of an NFT project. It contains an example of a simple collectible and an advanced one. It follows the ERC721 standards. Contracts contained:

- `AdvancedCollectible`: It creates a random collectible between 3 puppies
- `SimpleCollectible`: It creates the simplest NFT, following the ERC720 standards.

- [nft-demo]](#nft-demo)
  - [Summary](#summary)
  - [Prerequisites](#prerequisites)
- [Usage](#usage)
  - [Scripts](#scripts)
  - [Testing](#testing)
- [License](#license)

## Prerequisites

Please install or have installed the following:

- [nodejs and npm](https://nodejs.org/en/download/)
- [python](https://www.python.org/downloads/)
- [brownie](https://eth-brownie.readthedocs.io/en/stable/install.html)
- [ganache-cli](https://www.npmjs.com/package/ganache-cli)

# Usage

## Scripts

```bash
brownie run scripts/simple_collectible/deploy_and_create.py
```

This will deploy the "SimpleCollectible" contract, deploy some mock Chainlink contracts for you to interact with.

```bash
brownie run scripts/advanced_collectible/deploy_and_create.py
```

This will deploy the "AdvancedCollectible" contract, deploy some mock Chainlink contracts for you to interact with.

```bash
brownie run scripts/advanced_collectible/create_metadata.py
```

This will create the metadata for the "AdvancedCollectible" token already created.

```bash
brownie run scripts/advanced_collectible/create_uri.py
```

This will create the URI for the token to be assigned

```bash
brownie run scripts/advanced_collectible/set_tokenuri.py
```

This will link the uri created on the "create_uri" script.

## Testing

```
brownie test
```

# License

This project is licensed under the [MIT license](LICENSE).
