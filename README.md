# Cross-Chain NFT Marketplace

[![Solidity](https://img.shields.io/badge/Solidity-%5E0.8.0-blue)](https://docs.soliditylang.org/)
[![Hardhat](https://img.shields.io/badge/Hardhat-2.x-yellow)](https://hardhat.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-4.x-blue)](https://www.typescriptlang.org/)
[![LayerZero](https://img.shields.io/badge/LayerZero-Enabled-green)](https://layerzero.network/)

A decentralized NFT marketplace that enables cross-chain NFT trading using LayerZero protocol. This project allows users to list, buy, and sell NFTs across different blockchain networks.

## Features

- 🔄 Cross-chain NFT trading
- 🎨 NFT minting and listing
- 💰 Multi-chain payment support
- 🔐 Secure cross-chain message passing
- ⚡ LayerZero integration
- 🔍 NFT verification system

## Architecture

The project consists of two main components:

1. **NFT Contract**: Handles NFT minting and ownership
2. **Marketplace Contract**: Manages listings, sales, and cross-chain transactions

### Deployed Contract Addresses

#### Testnet Deployments

**NFT Contract:**
- Network: Avalanche Fuji
- Address: `0x025EF5a2d6AF68E229fC9A49681a64ce0787D520`
- [View on Snowtrace](https://testnet.snowtrace.io/address/0x025EF5a2d6AF68E229fC9A49681a64ce0787D520)

**Marketplace Contract:**
- Network: Ethereum Rinkeby
- Address: `0x6b49795FF24F2d23631d97E6fA235f9E2AF00911`
- [View on Etherscan](https://rinkeby.etherscan.io/address/0x6b49795FF24F2d23631d97E6fA235f9E2AF00911)

**LayerZero Endpoints:**
- Rinkeby: `0x5a6ef98aDcf9dF1903956cCfA46a00Bff6628FA0`
- Fuji: `0x819d5e4b469b428DC542b13a3319EDfFD58aC2E2`

## Prerequisites

- Node.js >= 14
- npm or yarn
- MetaMask or other Web3 wallet

## Installation

1. Clone the repository
```bash
git clone https://github.com/devincredible/crosschain-nft-marketplace.git
cd crosschain-nft-marketplace
```

2. Install dependencies
```bash
npm install
```

3. Create a `.env` file with your configuration
```env
PRIVATE_KEY=your_private_key
AVALANCHE_TESTNET_URL=your_rpc_url
RINKEBY_URL=your_rpc_url
ETHERSCAN_API_KEY=your_api_key
SNOWTRACE_API_KEY=your_api_key
```

## Development

### Compile Contracts
```bash
npx hardhat compile
```

### Run Tests
```bash
npx hardhat test
REPORT_GAS=true npx hardhat test # with gas reporting
```

### Deploy Contracts
```bash
npx hardhat run scripts/deploy.ts --network fuji # for NFT contract
npx hardhat run scripts/deploy.ts --network rinkeby # for marketplace contract
```

### Code Quality
```bash
# Lint TypeScript/JavaScript files
npx eslint '**/*.{js,ts}'
npx eslint '**/*.{js,ts}' --fix

# Format code
npx prettier '**/*.{json,sol,md}' --check
npx prettier '**/*.{json,sol,md}' --write

# Check Solidity contracts
npx solhint 'contracts/**/*.sol'
npx solhint 'contracts/**/*.sol' --fix
```

### Additional Commands
```bash
npx hardhat accounts
npx hardhat clean
npx hardhat node
npx hardhat coverage
```

## Technical Stack

- **Smart Contracts**: Solidity
- **Development Framework**: Hardhat
- **Cross-Chain Protocol**: LayerZero
- **Testing**: Mocha, Chai
- **Language**: TypeScript
- **Code Quality**: ESLint, Prettier, Solhint

## Security

- Smart contracts are designed with security best practices
- Cross-chain message passing is secured by LayerZero protocol
- Regular security audits are recommended before mainnet deployment

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Resources

- [LayerZero Documentation](https://layerzero.network/docs)
- [Hardhat Documentation](https://hardhat.org/getting-started/)
- [Solidity Documentation](https://docs.soliditylang.org/)
- [Avalanche Documentation](https://docs.avax.network/)