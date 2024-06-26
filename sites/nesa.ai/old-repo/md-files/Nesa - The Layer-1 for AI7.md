3/25/24, 11:40 AM Nesa - The Layer-1 for AI
https://www.nesa.ai/x/tokenization 1/3
Tokenization
DIGITAL ASSET
 Playground Technology Research Token Docs Developers DNA X3/25/24, 11:40 AM Nesa - The Layer-1 for AI
https://www.nesa.ai/x/tokenization 2/3
Nesa’s native asset, NES, is an essential part of how developers build on the blockchain
network for AI inference querying. To use Nesa for AI model querying, rollup developers
submit PayForQuery transactions on the network for a fee, denominated in NES.
Role of NES
Just as ETH is used on Ethereum-based rollups, developers can query their AI model
quickly through Nesa by using NES as a gas token and currency in addition to paying for
data availability.
To publish data on Nesa developers can submit PayForQuery
transactions. This is facilitated by queryStream, the method to
stream Nesa's Verification Layer results to the blockchain.
Each PayForQuery transaction is split into two parts: the inference query which includes
the data to be made available along with the namespace and signature, and the NES
executable payment transaction which includes a commitment to the data. The block data
is extended using erasure coding and then Merkelized into a data root commitment
included in the block header.
Nesa uses a standard gas-price prioritized mempool. This means that transactions with
higher fees will be prioritized by validators. Fees are comprised of a  at fee per transaction
and then a variable fee based on the size of each query in the transaction.
 Playground Technology Research Token Docs Developers DNA X3/25/24, 11:40 AM Nesa - The Layer-1 for AI
https://www.nesa.ai/x/tokenization 3/3
COPYRIGHT 2024 NESA FOUNDATIONGITHUB CAREERS TEAM TERMS PRIVACY CONTACT
 Playground Technology Research Token Docs Developers DNA X