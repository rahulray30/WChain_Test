# Sample Hardhat Project

This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a Hardhat Ignition module that deploys that contract.

## Contracts

### MockLiquidityPool

The `MockLiquidityPool` contract simulates a liquidity pool with basic functionalities such as adding liquidity, removing liquidity, swapping tokens, and getting exchange rates.

#### Functions:
- `addLiquidity(address token, uint256 amount)`: Adds liquidity for a specific token.
- `removeLiquidity(address token, uint256 amount)`: Removes liquidity for a specific token.
- `swap(address fromToken, address toToken, uint256 amount)`: Swaps a specified amount of one token for another.
- `getExchangeRate(address fromToken, address toToken)`: Returns the exchange rate between two tokens.
- `getLiquidity(address token)`: Returns the liquidity available for a specific token.

### MockToken

The `MockToken` contract is an ERC20 token with customizable decimals.

#### Constructor:
- `constructor(string memory name, string memory symbol, uint8 decimal)`: Initializes the token with a name, symbol, and decimal places.

#### Functions:
- `decimals()`: Returns the number of decimal places for the token.

## Running Tasks

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat ignition deploy ./ignition/modules/Lock.ts
```
