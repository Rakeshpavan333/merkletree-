# Merkle Tree
 Merkle Tree is used in the Bitcoin blockchain to verify the existence of a transaction in a way that conserves both space and time quite effectively .
 
Using a hash tree like a Merkle tree:

Significantly reduces the amount of data that a trusted authority has to maintain to proof the integrity of the data.
Significantly reduces the network I/O packet size to perform consistency and data verification as well as data synchronization.
Separates the validation of the data from the data itself -- the Merkle tree can reside locally, or on a trusted authority, or can itself reside on a distributed system (perhaps you only maintain your own tree.)  Decoupling the "I can prove the data is valid" from the data itself means you can implement the appropriate and separate (including redundant) persistence for both the Merkle tree and the data store.

Merkle trees provide a means of proving that integrity / validity of your data.
Merkle trees require little memory / disk space and proofs are computationally easy and fast.
Merkle tree proofs and management requires only a very small and terse amount of information to be transmitted across a network.
