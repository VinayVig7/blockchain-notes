The mechanism that achieves this agreement is called a consensus mechanism. Bitcoin uses a Proof of Work (PoW) consensus mechanism, but other blockchains might use Proof of Stake (PoS) or other mechanisms.

In Bitcoin's PoW system:

Miners compete to solve a cryptographic puzzle. The first miner to solve it gets to add a new block to the blockchain and broadcast it to the network.
Once the network agrees that this block is valid (following the consensus rules), it becomes part of the blockchain.
Consensus Blocks in Bitcoin
If by "consensus blocks" you're referring to blocks that are accepted as part of the main chain, here's a more detailed explanation:

Valid blocks are those that follow the consensus rules (e.g., valid transactions, proper proof of work, no double-spending).
These valid blocks are added to the blockchain and accepted by the network as the true, agreed-upon state of the blockchain.
When a block is added to the main chain, it is considered a consensus block, because it reflects the network's agreement.



ORPHAN BLOCKS
In a decentralized network like Bitcoin, multiple miners are constantly trying to add new blocks to the blockchain. Occasionally, two miners might solve a block at nearly the same time. This creates a temporary situation where two competing valid blocks are broadcast to the network. Nodes in the network may initially accept both blocks as part of the blockchain, leading to a temporary fork.

Eventually, one of the chains will become longer (or have more proof of work), and the network will decide to adopt this longer chain as the valid chain.
The block that is on the shorter chain becomes an orphan block because it is no longer part of the main chain.

When a block becomes an orphan block in the Bitcoin network, the transactions that were included in that block are not lost. Instead, they are reinserted into the mempool (transaction pool), where they remain until they are included in a valid block on the main chain