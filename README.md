# BlockChain
Code Strategy:
1. store transactions in a vector
2. each transacion is identified by its ID, and consists of ID, size in bytes and fee in BTC.
3. each block is identified by index and consists of transactions it includes, hashvalue and reward the block has earned.
4. sort the stored transactions by descending order of fee
5. add transactions to the block until the size of the block is reached to max block size
6. calculate reward by adding the fee of the transaction.
7. maximum reward will be the flat reward for a block(12.5 BTC) + reward of added  fees.

