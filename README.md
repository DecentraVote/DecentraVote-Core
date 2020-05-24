# DecentraVote-Core

DecentraVote is an electronic voting protocol enabling tamper-proof decision making in general meetings and other governing bodies of organizations.

DecentraVote-Core published in this repository provides common functionality agnostic to legal form and jurisdiction. It can be used to build custom e-voting applications tailored to cooperatives, associations and other organisations, which are subject to specific statutes and legal provisions.

More details can be found in the [whitepaper](Whitepaper_DecentraVote.pdf)

## Blockchain and Smart Contracts
The DecentraVote protocol is compatible with any blockchain network using the EVM. Smart contracts manage the accounts of members of the governing bodies and support the conduct of votes. Members use one-time Ethereum accounts to cast votes and thereby remain anonymous.

## Advanced Cryptography
In order to legitimate one-time accounts members provide zk-SNARK proofs generated by the DApp in their browser. To avoid using accounts which can be traced back to members, the transactions registering one-time accounts are submitted using a relay network. Votes cast are kept secret until the counting starts by the means of elliptic curve cryptography.

## Decentralized App
The DApp as well as any texts and files it uses are hosted by a decentralized storage. The decentralized storage commits the hash of everything it persists on the blockchain. The DApp running in the browser computes the hash of any content loaded from the decentralized storage and compares it with the hash stored on the blockchain.
