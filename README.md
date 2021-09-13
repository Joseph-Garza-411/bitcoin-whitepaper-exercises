# Bitcoin Whitepaper Exercises

In these exercises, you will learn about blockchains from the perspective of the [original Bitcoin Whitepaper](https://bitcoin.org/en/bitcoin-paper).

* [Hashing](hashing/README.md)
* [Transactions](transactions/README.md)
* [Wallet](wallet/README.md)
* [Proof of Work](pow/README.md)
* [Incentives](incentives/README.md)

 ## Bitcoin Whitepaper Exercises 

In this exercise, you will practice writing code to create blocks, compute block hashes, and verify blocks based on those hashes. 

## Part I: 

You are provided lines of text from a poem, and you should loop through them and add each line as its own block of data to the provided blockchain. 

Define a ['createBlock(...)'] function which takes the text for its data, creates an object for the block, and computes its hash, finally returning the block object. Insert this object into the ['blocks'] array for the blockchain. 

Each block should have the following fieds: 

* ['index']: an incrementing number that's the 0 based position of the new block within the blocks array; the genesis block has ['index']of [0], so the next block will have ['index'] of [1]

* ['prevHash']: the value of the [hash] field from the last block in the [blocks] arrray. 

* ['data']: the string value passed into [createBlock(...)]

* `timestamp`: the numeric time stamp `from Date.now`

* `hash`: the SHA256 hash of the block's other fields (`index`, `prevHash`, `data`, and `timestamp`)

Verify that your blockchain includes all 8 lines of the poem, each as separate blocks,for a total of 9 blocks including the genesis block. 