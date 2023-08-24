---
title: "Bitcoin WhitePaper Simplified"
seoTitle: "Bitcoin WhitePaper Simplified"
datePublished: Fri Aug 26 2022 08:22:45 GMT+0000 (Coordinated Universal Time)
cuid: cl7a7hnws00pg9ynvgew10izp
slug: bitcoin-whitepaper-simplified
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1661502139519/pDaGBLX_d.webp
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1661502148924/HGtb0PP0g.webp
tags: hashnode, bitcoin, cryptocurrency, hashnodecommunity

---

Bitcoin Whitepaper is the first document through which people got to know about Bitcoin. [**Bitcoin Whitepaper**](https://bitcoin.org/bitcoin.pdf) was published in 2008 by Satoshi Nakamoto.

Bitcoin Whitepaper is a 9-page document in which Satoshi explained What Bitcoin is and how this work in detail. If you want you can check the whitepaper here.

Bitcoin Whitepaper has a lot of details about Bitcoin and it gets a little complex for some people to understand who do not have a lot of technical knowledge. So to help them I have come up with this article where I will explain the Bitcoin Whitepaper in a simplified way.

There are 9 different parts in the Bitcoin Whitepaper as follows:

1. Introduction
2. Transactions
3. Timestamp Server
4. Proof-of-Work
5. Network
6. Incentive
7. Reclaiming Disk Space
8. Simplified Payment Verification
9. Combining and Splitting Value
10. Privacy
11. Calculation

We will go through each part one by one.

# 1. Introduction

In this part, Satoshi Nakamoto talks about the central authority in the traditional payment system. He told that all the major transactions that happen today on the internet involve a third party, e.g. banks. Transactions on the internet were relying completely on financial institutions which served as third parties to process electronic payments. Here in this model, all the transaction that happens is based on trust. The seller trusts the bank and the bank trusts us and in this way the transaction happens. The bank has all our information and we trust the bank with our information.

He also told that the chances of fraud in this traditional model are as one can fake his/her identity. The chances of fraud can be avoided by using a physical currency. But not every time we can use the physical currency. So there is a need for a mechanism to carry out transactions on the internet without a trusted third party.

There is a need for an electronic payment system that is based on cryptographic proof and not trust, which will allow two different parties to transact directly without the need for a third party.

# 2. Transactions

In this part of the paper, he talks about how the transaction happens in bitcoin.

Whenever a transaction happens in bitcoin, all the transactions are recorded in a ledger. A ledger is basically like a page where all the transaction details are recorded. In the blockchain, this is maintained as a digital ledger. Here the transactions are recorded in the form of digital signatures. Digital signatures were basically hashes. Later in the article, we are going to know what are hashes.

The main issue in bitcoin was how to prevent double-spending. Let me explain what double spending is, suppose one person has to give Rs100 to two persons each but he only has one note. Now he could make a copy of the 100 rupee note and give one each to both of them. Now I know this is not possible but assume it just for the sake of example. Now since bitcoin is a digital currency, one hacker can disrupt the blockchain network and can send a copy of any previous transaction to make it look legitimate.

Now the common solution for this is to introduce a trusted central authority that checks every transaction and finds out the double-spending if it happens. But still, here the entire system was dependent on the central authority whereas bitcoin’s purpose was to remove the central authority and to make the system decentralized.

To solve this problem he proposed a solution that only the early transactions will be considered. So even if the same transaction happens later it won’t be counted. But here since there is no central authority to keep a check on the transactions, he mentioned that all the transactions must be publicly announced and people all around the world will contribute to verifying the transaction.

# 3. Timestamp Server

Now here he introduced the Timestamp Server. Since the previous part, we got to know that the earliest transaction would be counted as valid. So, now in the ledger whenever a transaction happens the time stamp will be recorded. In this way, it would be easier to find out which transaction happened first.

# 4. Proof of Work

Now the proof of work here is a very important part of the bitcoin blockchain. Proof of work is used to identify whether a ledger is valid or not.

Now here we will get to know about Hash. A hash is used to check the validity of a ledger. Let us take an example and understand what is a hash.

Suppose you are making a cake. You take all the ingredients like butter, flour, egg, baking powder, etc. Now you mix them and make the cake batter. Now here the cake batter is the items in the ledger. Now you require an oven to make the cake. Now here the oven is the cryptographic function. Now after baking, you get the yummy cake which is the Hash. Now simplifying it when you put the items of the ledger into the cryptographic function you get the hash. Hash contains all the data in the ledger in the form of a combination of numbers and letters.

Look at this image to understand it more clearly.

![2.avif](https://cdn.hashnode.com/res/hashnode/image/upload/v1661501464033/0y8_7btok.avif align="left")

Now, any changes you make in the ledger the hash code changes. This prevents hackers from accessing all the blocks in the blockchain.

Now, the very interesting thing about hash is that it cant be reversed. For example, you cannot get the ingredients back from the cake because it is irreversible. This prevents hackers from accessing the information on the ledger.

Now not every hash is valid. To find the valid hash there is no other way rather than guessing. All the nodes around the world guess the hash. Bitcoin follows a specific protocol the valid hash must contain an n-number of zeroes in the beginning.

# 5. Network

Here he explains the steps in which bitcoin’s blockchain network functions.

1. First, the new transactions are publicly announced and sent to all the nodes(computers).
2. Each node collects the new transaction and adds it to the ledger.
3. Then each node tries to guess the hash and when one node finds the valid hash it broadcasts it to the other nodes.
4. All the nodes then check the ledger and only accept it if all the transactions are valid and double-spending has not happened.
5. Then all the nodes accept the ledger by working on a new ledger/block which includes the valid hash of the previous block and thus it forms a chain.

As I told you above in bitcoin’s blockchain that the longest chain is considered to be the correct one and the nodes keep on extending it. Satoshi here proposed a solution what if two nodes broadcasted two different versions of the ledger/block at the same time? Then two versions will be kept until one of the ledgers gets longer and then the shorter one will be cancelled out and the longer one continues.

# 6. Incentive

When miners(nodes) find the valid hash, then they confirm the early transaction and then it is considered a valid transaction.

When they validate a transaction they get rewarded an incentive in the form of coins which are collected from the transaction fees. This is done to encourage the nodes to stay honest.

# 7. Reclaiming Disk Space

Here he explains the parts of the chain where items can be deleted to save disk space. I am not going very deep into this because this is a bit technical. If you still want to read it you can check it out in the whitepaper.

# 8. Simplified Payment Verification

Here he explains that the payments can be verified without going through the entire ledger rather it happens through branches known as Merkle Branch.

This helps the payment verification process to happen in a short period of time.

# 9. Combining and Splitting Values

Here he explains how is a transaction defined in bitcoin’s blockchain. Not every cent transferred is considered a transaction and recorded in a ledger. A single input from a previous large transaction or multiple small transactions combined to form a large transaction is called a transaction.

# 10. Privacy

When a transaction happens in the traditional model, the bank acts as a central authority and our information is with the bank. But in bitcoin, since there is no central authority, all the transactions are publicly announced. But do not worry as our name does not get recorded in the ledger. Even if someone gets access to the ledger they won’t get much info.

# 11. Calculations

This part of the paper explains the calculation that prevents a hacker from creating an alternate chain faster than the honest chain. This is very technical and we are not going deep into this.

# Conclusion

Now, I hope you have got a clear idea about the Bitcoin Whitepaper. Now still if you have any doubts regarding this then ask them in the comments and I will reply to them. Thanks for reading 😊
