# Sushi - X - Swap

Sushi - X - Swap enables cross chain transfers and swaps for the sushiswap. 

It supports swaps from both Trident and Legacy AMM. 

The bridging solution used is Stargate.

User can choose to transfer or swap from both BentoBox or Wallet, or even both.

## Env

```sh
cp .env.example .env
```

## Test

```sh
yarn test
```

```sh
yarn test test/Greeter.ts
```

## Coverage

```sh
yarn test:coverage
```

<https://hardhat.org/plugins/solidity-coverage.html#tasks>

## Gas

```sh
yarn test:gas
```

<https://github.com/cgewecke/hardhat-gas-reporter>

## Lint

```sh
yarn lint
```

## Watch

```sh
npx hardhat watch compile
```

## Deployment

### Local

Running the following command will start a local node and run the defined deploy script on the local node.

```sh
npx hardhat node
```

### Mainnet

```sh
yarn mainnet:deploy
```

```sh
yarn mainnet:verify
```

```sh
hardhat tenderly:verify --network mainnet ContractName=Address
```

```sh
hardhat tenderly:push --network mainnet ContractName=Address
```

### Ropsten

```sh
yarn ropsten:deploy
```

```sh
yarn ropsten:verify
```

```sh
hardhat tenderly:verify --network ropsten ContractName=Address
```
