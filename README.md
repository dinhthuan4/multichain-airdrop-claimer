### README

---

# Multi-Chain Airdrop Claimer Bot

## Overview

The **Multi-Chain Airdrop Claimer Bot** is a Python-based tool for claiming airdrops on both **Solana** and **Ethereum/EVM-compatible chains** (e.g., Ethereum, Binance Smart Chain, Polygon). The bot checks eligibility and claims airdrops automatically if eligible, making it easy to participate in multiple airdrops across different blockchains.

### Features

- **Supports Solana and Ethereum**: Works on Solana, Ethereum, and EVM-compatible chains.
- **Eligibility Check**: Verifies if the wallet is eligible for each airdrop.
- **Claim Execution**: Automatically claims airdrops for eligible addresses.
- **Transaction Logging**: Logs transaction IDs for all successful claims.

### Prerequisites

1. Python 3.x
2. Libraries: `solana-py` and `web3.py`
3. RPC Provider for Solana and Ethereum/EVM networks (e.g., Infura, Alchemy, or your own node)
4. Wallets for both Solana and Ethereum/EVM networks.

Install the necessary libraries with:

```bash
pip install solana web3
```

### Usage

#### Step 1: Configure the RPC URLs and Wallet Keypairs

- **solana_rpc_url**: Set to your Solana RPC provider endpoint.
- **eth_rpc_url**: Set to your Ethereum provider (e.g., Infura).
- **solana_wallet_keypair**: Provide your Solana wallet keypair.
- **eth_private_key**: Private key for your Ethereum wallet.

#### Step 2: Define Airdrop Contract Addresses

Add contract addresses for the airdrops you want to claim, specifying the blockchain for each contract.

Example configuration:
```python
airdrop_contracts = {
    'solana': [
        "SOLANA_AIRDROP_CONTRACT_ADDRESS_1",
        "SOLANA_AIRDROP_CONTRACT_ADDRESS_2"
    ],
    'eth': [
        "ETH_AIRDROP_CONTRACT_ADDRESS_1",
        "ETH_AIRDROP_CONTRACT_ADDRESS_2"
    ]
}
```

#### Step 3: Run the Script

Run the script using:

```bash
py multi_chain_airdrop_claimer.py
```

The bot will check eligibility and claim eligible airdrops for each specified contract.

### Important Notes

- **Contract ABI for Ethereum**: Ensure the correct ABI is loaded for each Ethereum contract in the script.
- **Airdrop Eligibility**: Customize eligibility checks based on contract requirements.
- **Terms of Use**: Confirm that automation is permitted for

 each airdrop to avoid violations.

### Limitations

- **Manual ABI Input**: The bot currently requires ABI for each Ethereum airdrop contract.
- **Placeholder Functions**: Replace placeholders with actual instructions for contract interaction.

### Future Enhancements

- **Automated ABI Loading**: Allow loading ABIs directly from Etherscan or another source.
- **Additional Chains**: Add support for other chains (e.g., Polygon, BSC) with minimal changes.

---

This tool provides a starting point for automating airdrop claims across multiple blockchains. Let me know if you have any questions or would like to add further customization options!print('jzlkugg')