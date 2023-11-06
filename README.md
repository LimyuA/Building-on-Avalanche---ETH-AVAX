# DefiToken

## ERC20 Token Contract

### Introduction
This repository contains a Solidity smart contract named `ERC20`. This contract implements the ERC20 standard interface for a basic fungible token. Below are the details of the functionalities and how to use them.

### Contract Details
- **Name**: Solidity by Example
- **Symbol**: SOLBYEX
- **Decimals**: 18

### Functions

#### `transfer`

function transfer(address recipient, uint amount) external returns (bool)

Transfers a specified amount of tokens from the sender's account to the recipient's account.

#### `approve`

function approve(address spender, uint amount) external returns (bool)

Allows the spender to withdraw from the sender's account, multiple times, up to the amount.

#### `transferFrom`

function transferFrom(address sender, address recipient, uint amount) external returns (bool)

Transfers a specified amount of tokens from the sender's account to the recipient's account.

#### `mint`

function mint(uint amount) external

Mints a specified amount of tokens and assigns them to the sender's account.

#### `burn`

function burn(uint amount) external

Burns a specified amount of tokens from the sender's account.

### Events

- `Transfer(address indexed from, address indexed to, uint value)`
- `Approval(address indexed owner, address indexed spender, uint value)`

### Usage

#### Deployment

To deploy this contract, follow these steps:

1. Deploy the contract using a Solidity compatible platform or an Ethereum development environment like Remix.

#### Interacting with the Contract

- Use a wallet or a contract to interact with the functions provided by the ERC20 contract.

-----------------------------------------------------------------------------------------------------------------------------------

## Vault Contract

### Introduction
This repository also contains a Solidity smart contract named `Vault`. This contract manages the deposit and withdrawal of a specific ERC20 token while minting and burning corresponding shares. Below are the details of the functionalities and how to use them.

### Functions

#### `deposit`

function deposit(uint _amount) external

Deposits a specified amount of tokens into the vault and mints corresponding shares to the depositor.

#### `withdraw`

function withdraw(uint _shares) external

Withdraws a specified amount of shares from the vault and burns the corresponding shares, transferring the equivalent tokens to the withdrawer.
