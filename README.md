# ProofQuest -The Offline Data Marketplace (ODM) — Powered by TON

**Bridging the gap between real-world data and the digital economy.**
Collect, verify, and reward real-life information through a decentralized, Telegram-native data marketplace.

## 🚀 Overview

**ProofQuest** transforms real-world interactions into verifiable, blockchain-powered data.

It's a decentralized platform that connects organizations needing verified offline data (e.g. real-world observations, photos, product checks) with a community of contributors who can collect this data in exchange for TON-based rewards.

Participants access **ProofQuest** directly via a Telegram Mini App, where they can browse bounties, submit verifications, and get paid once their submissions are approved.

Our platform bridges the gap between real-world data and digital incentives.

## 💡 Problem

Access to high-quality offline data is limited, expensive, and centralized.
Companies rely on agencies or field teams to verify simple, real-world facts — creating slow and costly feedback loops.

There’s no global, decentralized way to request or supply verified, real-world data.

## 🌍 Solution

ProofQuest introduces a decentralized marketplace that turns real-world verification into on-chain missions:

### Organizations / Researchers:
Post verification tasks ("bounties") via a web dashboard.
Specify what data or photo is needed, describe the requirements, and fund the bounty using TON.

### Contributors (Users):
Access the bounties via a Telegram Mini App.
Pick a mission, capture the requested data (e.g., photo or form), and submit.
Once verified, they receive instant TON rewards via smart contract.

## 🧩 Example Use Cases

🛒 Retail product availability checks
🌿 Environmental monitoring and reports
🏪 Brand compliance and shelf audits
🚧 Civic data: infrastructure or safety reports
🗺️ Crowdsourced geodata collection


## 🔄 Future Expansion

In future releases, ProofQuest will evolve into a two-way marketplace:
not only can organizations request data, but users will also be able to propose valuable offline data (e.g. local observations, environmental reports, product sightings).

These user-proposed datasets can attract buyers, creating a fully decentralized data supply and demand ecosystem.

## 🎮 Additional Upcoming Features

**Gamification:** contributors can level up, earn badges, and unlock higher-tier missions.

**Referral System:** invite friends to join and earn bonus TON rewards for verified referrals.

**Leaderboard:** global and local leaderboards to showcase top contributors and motivate engagement.

## 🔗 Key Features

### 🧠 For Companies / Researchers

- Create and fund verification bounties in TON
- Define photo or data requirements
- Review and approve submissions
- Export verified data via dashboard or API

###📱 For Contributors (via Telegram Mini App)

- Secure login via Telegram + TON Connect
- Browse active bounties or nearby missions
- Submit photo or data evidence directly from Telegram
- Receive instant TON payments after verification

## 🧱 Architecture

### Core Components
- Frontend (Web App): XX dashboard for posting and managing bounties

- Telegram Mini App: TON-integrated interface for contributors

- Smart Contracts: TON contracts handle escrow and automated reward payouts

- Backend API: Stores metadata, image references (IPFS), and handles verification logic

- AI Verification Engine: Processes image submissions using computer vision and ML models (e.g. object detection, photo integrity, and metadata checks)

- Storage Layer: IPFS or cloud service for storing verified submissions

### Workflow

1. Organization posts and funds a bounty → TON smart contract locks funds
2. Bounty appears in Telegram marketplace
3. User submits data → processed by the AI Verification Engine for authenticity and content validation
4. Optional human review if AI confidence < threshold
5. Upon approval → smart contract releases TON reward

### 💎 TON Integration

### ⚙️ Tech Stack

## 🧱 Getting Started (Hackathon Prototype)

## 🤝 Team & Credits
Built for the TON Hackathon 2025 in 42 Berlin
Powered by ODM Protocol (Offline Data Marketplace)
Team: [Your Team Name]
Members: [faramirezs](https://github.com/faramirezs), [tpandya42](https://github.com/tpandya42), [mainibet](https://github.com/mainibet), [educhigon](https://github.com/educhigon)

✨ “Bringing the offline world on-chain — one photo, one bounty, one TON at a time.” ✨ 
