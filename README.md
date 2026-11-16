# AbaTrust
**USDC escrow and on-chain reputation for fabric and garment trading in
Aba, Nigeria.**

AbaTrust is a prototype application aimed at reducing payment and trust
risks in bulk fabric transactions across Aba's fabric and garment
markets, especially Ariaria and related wholesale clusters.

## The problem

Bulk fabric deals often depend on personal relationships and informal
trust:

-   *Buyers* may pay upfront and receive counterfeit, substituted, or
    poor-quality fabric.
-   *Sellers* may deliver goods and face delayed payment or
    non-payment.
-   *Cash and bank transfers* can introduce security, cost, and
    settlement friction.
-   *Proof of delivery and trading history* can be difficult for new
    counterparties to verify.

These barriers frequently prevent otherwise valuable transactions from taking place.

## The Proposed Solution

AbaTrust explores a simple **USDC escrow + on-chain reputation** workflow built for the Arc ecosystem:

1. A seller creates a deal specifying fabric type, quantity, USDC price, and delivery terms.
2. The buyer locks the agreed USDC amount in escrow.
3. The seller fulfills the order and provides delivery evidence (photos or an inspection step can be used as supporting confirmation).
4. Once delivery is confirmed under the agreed terms, the escrow releases the funds to the seller.
5. Completed transactions contribute to each party’s public on-chain reputation.

The goal is a safer and more transparent way for buyers and sellers to transact — even when they do not already know one another.

## Demo

- **Live application:** [https://startling-mandazi-b572ed.netlify.app/](https://startling-mandazi-b572ed.netlify.app/)
- **Alternative deployment:** [https://6aeacdcc04bd8dad621ff2aa--startling-mandazi-b572ed.netlify.app/](https://6aeacdcc04bd8dad621ff2aa--startling-mandazi-b572ed.netlify.app/)
- **YouTube demo:** [https://www.youtube.com/watch?v=9L8Gt_dhPzk&t=166s](https://www.youtube.com/watch?v=9L8Gt_dhPzk&t=166s)

## Why Arc and USDC?

The project is designed around stable-value USDC settlement and Arc’s blockchain environment. The aim is to make payment settlement predictable while supporting verifiable transaction history.

> **Important:** Before using this project with real funds, carefully verify the network, token contract, escrow contract, security assumptions, and deployment status in the source code and configuration. Do not treat a demo as an audited or production-ready financial service.

## Current Status

AbaTrust is a **prototype**. The workflow described above represents the project’s intended functionality. Please refer to the live demo and source code for the features currently implemented.

## Technology

Built for the Arc ecosystem with USDC-based settlement.  
*(Add the exact frameworks, libraries, wallet integrations, smart-contract language, and tooling used by this implementation here.)*

## Getting Started

Local installation instructions will be added once the full source code and build configuration are available in this repository.

Example setup (to be updated with actual commands):

bash
# Clone the repository
git clone <your-repository-url>
cd <repository-folder>

# Install dependencies
npm install

# Start the development server
npm run dev


## Roadmap

- [ ] Complete and document the full buyer/seller deal flow
- [ ] Integrate and test USDC escrow on the intended Arc network
- [ ] Add clear delivery confirmation and dispute-resolution rules
- [ ] Implement transparent on-chain reputation updates for completed deals
- [ ] Add automated tests and security review
- [ ] Conduct usability testing with fabric traders and gather feedback

## Contributing

Contributions, testing, and practical feedback are welcome.  

If you are a developer, please open an issue describing the improvement or submit a pull request with a clear summary and test notes.

## Disclaimer

AbaTrust is a prototype currently under development. It does not guarantee product quality, delivery, payment, or dispute resolution. Always verify the current implementation and smart-contract security before using real funds.
