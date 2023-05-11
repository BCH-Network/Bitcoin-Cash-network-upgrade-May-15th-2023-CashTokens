# Bitcoin Cash network upgrade May 15th 2023 [CashTokens](https://cashtokens.cash/)
BitcoinCash Hardfork - Important update information (CASHTOKENS)

### Changelog:
- Most notably, the [CashTokens](https://cashtokens.cash/) upgrade which enables advanced abstraction in script and covenant designs, as well as conventional token and NFT usecases.
- P2SH32, which allows for more cryptographically secure transactions.
- Other minor improvements that cleans up the ruleset.

### For node operators, upgrade to the latest version of a compatible node:
- Compatible, released: Bitcoin Cash Node
- Yet to release a compatible version: Bitcoin Unlimited, Bitcoin Verde, BCHD, Knuth, Flowee the Hub

#### This update enables two new primitives on Bitcoin Cash: fungible tokens and non-fungible tokens.

>A token is an asset – distinct from the Bitcoin Cash currency – that can be created and transferred on the Bitcoin Cash network.

>Non-Fungible tokens (NFTs) are a token type in which individual units cannot be merged or divided – each NFT contains a commitment, a short byte string attested to by the issuer of the NFT.

>Fungible tokens are a token type in which individual units are undifferentiated – groups of fungible tokens can be freely divided and merged without tracking the identity of individual tokens (much like the Bitcoin Cash currency).

## Wallet for CashTokens
[CashTokens.cash](https://cashtokens.cash/) - [The first official BCH wallet that supports CashTokens](https://cashtokens.cash/)

### What is CashTokens and why is it promising?
CashTokens are a Bitcoin Cash virtual machine-enforced scheme for issuing, validating, and redeeming tokens. Tokens can be issued either by a trusted entity or by a Bitcoin Cash covenant configured to behave as a corporation and issuing its own tokens. CashTokens is better understood as adding internal state (programmatic power) and inter-contract communication to Bitcoin Cash contracts / transactions

[CashTokens](https://cashtokens.cash/) has already "locked-in" for implementation in November 2022, and will go live on the main network in the BCH network upgrade in May 2023. Consumer facing wallet integrations and apps should follow.

>[BCH CashTokens](https://cashtokens.cash/) magnifies the power of smart contracts on Bitcoin Cash enormously to close or equivalent to EVM chains like Ethereum, while retaining low fees at scale with a >1 000x scaleability advantage over those competitors.

### How is it different to SLP (Simple Ledger Protocol) tokens?
SLP tokens was a previous somewhat-similar implementation of tokens on BCH. CashTokens is distinct from SLP in several ways:

- Miner validation: Crucially, SLP tokens were not miner validated (they were built at a layer above the protocol), while BCH tokens are miner validated (they are native to the protocol). This means that SLP token transactions received by apps (e.g. wallets) had to check the entire history of each token to verify whether or not they were authentic. The more popular a token became, the slower the token apps became in response because the history of transfers to check got longer and longer. This problem was an even worse burden for SLP infrastructure, which had the same problem for EVERY kind of SLP token simultaneously. This meant much infrastructure was not high performing or well-maintained. In contrast, CashTokens transactions are valid by default if a wallet receives them (just as Bitcoin Cash transactions are) because nodes would not broadcast them and miners would not mine them in the first place if they weren't. Therefore successful CashTokens growth will not be hampered by a self-limiting negative feedback loop in the same way as SLP tokens were. No extra infrastructure for token validating is required either.
- Power: SLP tokens covered a far more limited set of functionality (token creation, transfers, burning & dividend payments). CashTokens has the same power, but also generic power to do many things beyond that (such as communication between BCH controlling contracts). This suggests that many things can and will be built with CashTokens to drive engagement that were not even possible with SLP.
- Problems with non-integrated software: SLP tokens could be accidentally burned by non-supporting BCH software - leading to frustrated users and ecosystem wide issues. CashTokens cannot be accidentally received (or burnt / lost) by wallets and applications that are not aware of it.

### What about a free distribution of CashTokens to BCH holders?
Yes, that was the plan. The first token after the network update on May 15 will be created Bitcoin Cash Xenoblast and partially distributed to active BCH addresses.
A total of 16,749,565,000 BCHX will be distributed to 35,000 addresses (478,559 BCHX per address)
You can read more about the terms of the airdrop here: https://bch.network/en/BitcoinCash-AirDrop-May-15-2023-Claim-Free-BCHX-Tokens

### Is it possible to fork the Bitcoin Cash network after the hardfork?
This possibility persists, but is currently supported by only a small fraction of developers, about 20%.
