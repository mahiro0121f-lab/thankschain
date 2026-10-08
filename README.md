# ThanksChain
![ThanksChain logo](assets/logo.png)

**Send on-chain thank-you cards with a small SOL tip attached**

## Overview
ThanksChain is a simple web app where users send digital thank-you cards to friends, with an optional small SOL tip bundled in. Each card is minted as a lightweight NFT so the recipient keeps it as a memory. It's built to be the easiest possible way to try sending value and NFTs on Solana.

## Problem
Sending crypto and minting NFTs still feels technical and intimidating for newcomers. Wallets, gas, mint addresses, and transaction signing create friction that scares beginners away before they ever experience what crypto can do.

## Solution
A single-page app that lets anyone mint and send a thank-you card NFT with an attached tip in under a minute. No jargon, no complex steps, just connect, write, and send.

## Features (MVP)
- Connect wallet (Phantom) with one click
- Pick a card design and write a short message
- Attach an optional SOL tip (fixed small amounts like 0.01 / 0.05 SOL)
- Mint the card as an NFT sent directly to the recipient's wallet
- Simple gallery page to view received cards

## Tech Stack
- Next.js
- Solana Web3.js
- Metaplex NFT standard
- Phantom Wallet Adapter
- Solana Devnet

## How It Works

```
[User] --connect--> [Phantom Wallet]
   |
   v
[Pick Card + Write Message + Choose Tip]
   |
   v
[Next.js App] --build tx--> [Solana Devnet]
   |                              |
   |                      mint NFT (Metaplex)
   |                      transfer SOL tip
   v
[Recipient Wallet] <--- NFT + Tip
   |
   v
[Gallery Page: view received cards]
```

The app builds a transaction that mints a lightweight NFT via the Metaplex standard and, if selected, transfers a small fixed amount of SOL to the recipient, all in one user-approved action on Solana Devnet.

## Roadmap
- Add mainnet support with real SOL amounts
- Let users create custom card designs/templates
- Add social sharing so cards can be posted publicly

## Pitch
- [Pitch deck (PDF)](docs/pitch.pdf)
- [Pitch script](docs/pitch-script.md)

## Team
- [Name] — Role (placeholder)
- [Name] — Role (placeholder)
- [Name] — Role (placeholder)

Built for the Colosseum hackathon.

---

🎬 Pitch video: [docs/pitch-video.mp4](docs/pitch-video.mp4)
