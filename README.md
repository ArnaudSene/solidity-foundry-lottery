# Proveably Random Raffle Contracts

## About

This code is to create a proveably random smart contract lottery.

- Use [Chainlink VRF](https://vrf.chain.link/) to [get a random number](https://docs.chain.link/vrf/v2/subscription/examples/get-a-random-number)
- Use [Chainlink Automation](https://dev.chain.link/products/automation) to start the draw

## How it works?

1. Users can enter by paying for a ticket
   1. The ticket fees are going to go to the winner during the draw
2. After X period of time, the lottery will automatically draw a winner
   1. And this will be done programmatically
3. Usind Chainlink VRF & Chainlink Automation
   1. Chainlink VRF -> Randomness
   2. Chainlink Automation -> Time base trigger

## Usage

> Required
> Rename `sample-env` by `.env` and replace with the approrpiate values

### Test 
```shell
make help
```
```
Usage:
  make deploy [ARGS=...]
    example: make deploy ARGS="--network sepolia"

  make fund [ARGS=...]
    example: make deploy ARGS="--network sepolia"
```



### Deploy
local chain (Anvil)
```shell
make deploy
```
Sepolia testnet
```shell
make deploy ARGS="--network sepolia"
```

### Install dependencies
```shell
make install
```

### Build
```shell
make build
```

### Test
```shell
make test
```