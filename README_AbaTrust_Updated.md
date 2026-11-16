# AbaTrust

**USDC escrow and on-chain reputation for fabric and garment trading in
Aba, Nigeria.**

AbaTrust is a prototype application aimed at reducing payment and trust
risks in bulk fabric transactions across Aba's fabric and garment
markets, especially Ariaria and related wholesale clusters.

## The problem

Bulk fabric deals often depend on personal relationships and informal
trust:

-   **Buyers** may pay upfront and receive counterfeit, substituted, or
    poor-quality fabric.
-   **Sellers** may deliver goods and face delayed payment or
    non-payment.
-   **Cash and bank transfers** can introduce security, cost, and
    settlement friction.
-   **Proof of delivery and trading history** can be difficult for new
    counterparties to verify.

These barriers can prevent otherwise valuable transactions from
happening.

## The proposed solution

AbaTrust explores a simple **USDC escrow + reputation** workflow built
for the Arc ecosystem.

1.  A seller creates a deal with the fabric type, quantity, USDC price,
    and delivery terms.
2.  The buyer locks the agreed USDC amount in escrow.
3.  The seller fulfills the order and provides delivery evidence. The
    parties may use photos or an inspection step as supporting
    confirmation.
4.  Once delivery is confirmed under the agreed terms, the escrow
    releases the funds to the seller.
5.  A completed transaction can contribute to each party's public
    on-chain reputation.

The intended result is a safer and more transparent way for buyers and
sellers to transact, including when they do not already know one
another.

## Demo

-   **Live application:** https://startling-mandazi-b572ed.netlify.app/
-   **Alternative deployment:**
    https://6aeacdcc04bd8dad621ff2aa--startling-mandazi-b572ed.netlify.app/
-   **YouTube demo:** https://www.youtube.com/watch?v=9L8Gt_dhPzk&t=166s

## Why Arc and USDC?

The project is designed around stable-value USDC settlement and Arc's
blockchain environment. The goal is to make payment settlement
predictable and to support verifiable transaction history.

> Before using this project for real funds, verify the network, token
> contract, escrow contract, security assumptions, and deployment status
> in the source code and deployment configuration. Do not treat a demo
> as an audited or production-ready financial service.

## Current status

AbaTrust is a prototype. The workflow described here represents the
project's intended functionality. Refer to the live demo and source code
for the features currently implemented.

## Technology

The project is intended for the Arc ecosystem and USDC-based settlement.
Add the exact frameworks, libraries, wallet integrations, smart-contract
language, and tooling used by this implementation here.

## Getting started

Local installation instructions are not included yet because the source
repository and its framework/build configuration have not been provided.

Once the source code is in this repository, replace this section with
the actual commands, for example:

``` bash
# Clone the repository
git clone <your-repository-url>
cd <repository-folder>

# Install dependencies (use the command for your package manager)
npm install

# Start the development server (replace with the project's actual command)
npm run dev
```

Check the project's `package.json` or equivalent configuration and
replace these example commands with the actual setup instructions before
publishing them as verified steps.

## Roadmap

-   [ ] Complete and document the buyer/seller deal flow.
-   [ ] Integrate and test USDC escrow on the intended Arc network.
-   [ ] Add clear delivery confirmation and dispute-resolution rules.
-   [ ] Implement transparent reputation updates for completed deals.
-   [ ] Add automated tests and security review.
-   [ ] Test usability with fabric traders and gather feedback.

## Contributing

Contributions, testing, and practical feedback are welcome. If you are a
developer, please open an issue describing the improvement or submit a
pull request with a clear summary and test notes.

## Disclaimer

AbaTrust is a prototype/project in development, not a guarantee of
product quality, delivery, payment, or dispute resolution. Verify the
current implementation and smart-contract security before using real
funds.
