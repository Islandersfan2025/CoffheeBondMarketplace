# CoffheeBondMarketplace
Demo of Coffhee Finance's bond trading platform.

The Coffhee Finance Infrastructure
The Confidential Hub (Arbitrum/Robinhood Chain + Fhenix):
The core of the ecosystem resides on Arbitrum, utilizing Fhenix’s FHE (Fully Homomorphic Encryption) coprocessor. This "Confidential Hub" hosts the ERC-3475 "Golden Copy" of the debt. It enables the encryption of sensitive financial data—such as principal amounts, individual yields, and institutional identities—allowing the blockchain to perform math on the debt while it remains encrypted.

The Liquid Spoke Model (Multichain):
Instead of siloed liquidity, Coffhee utilizes a "Spoke" architecture. While the complex bond logic lives on the Hub, ERC-1155 "Receipt NFTs" are provisioned to high-traffic chains like Base, BNB Chain, and Robinhood Chain. This allows retail traders to buy and sell bond positions in their native environment without needing to understand the underlying FHE encryption.

Multi-Class Debt Engine (ERC-3475):
The infrastructure moves beyond simple tokens to an Abstract Storage Bond standard. A single contract can manage infinite "classes" (types of bonds) and "nonces" (specific issuances). This allows Coffhee to support fixed-income, zero-coupon, and callable bonds within the same gas-efficient infrastructure, mimicking a sophisticated prime brokerage.

Permissioned Decryption & Sealing:
The platform features a native sealing protocol. When an authorized holder connects via the Terminal, the FHE coprocessor "seals" the private bond data specifically for that holder’s public key. This ensures that while the market sees a generic NFT, the owner sees their private amortized yield and maturity schedule directly in their interface.


