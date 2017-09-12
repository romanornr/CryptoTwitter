## 27 years before Bitcoin

The blockchain was introduced in 2008 together with Bitcoin and practically implemented in 2009.

In my last blog post: (https://medium.com/@romanornr/distributed-systems-and-byzantine-nodes-3ba99093eb02)
We looked at the concepts of understanding distributed system, the CAP theorem and Bitcoin using a Proof Of Work to achieve consensus. 

However other concepts existed before the invention of Bitcoin. Digital cash have always been in the mind of many cryptographers for decades. Early ideas date back as far as the early 80’s (Which is mind blowing if you think about the tech back then). 

### 1982 e-cash
In 1982 David Chaum proposed a scheme which uses blind signatures to build untraceable digital cash. 
Blind signatures simply explained without the details and I quote investopedia (Couldn not explain it simpler myself) “a type of digital signature where the message's content cannot be seen before it is signed” - investopedia 

A bank would issue for example digital cash by signing a blind and random serial number.  The user could use his digital token signed by the bank as currency. Yes, this was a centralized system which required the trust from the user. However this scheme had some flaws because the bank had to keep track of all used serial numbers. 

In 1990 David Chaum came up with an improved version he named e-cash which used private identification data to craft messages that would be sent to the bank. But he “solved” a problem you might have heard bouncing around “Double spend attack”. The scheme allows to detect double spending. You may wonder why I used the quotes on the word solved… The scheme detected it, but did not prevent it from happening. The idea was that if the same token was used twice at a different location, the identity of that user/attacker would be revealed. Worth to mention is that e-cash could only present a fixed amount of money. 

### 1997 hashcash
In 1997 Adam Back (Yes, he is currently the CEO of blockstream) introduced hashcash as a Proof Of Work system to control email spam which was a very creative idea. Hashcash was a simple but clever idea. If a user wanted to send an email they were required to compute a hash as a proof that they have spent time and computing resources before sending the email. 
If a spammer wanted to send hundreds or thousands of emails, it became infeasible to do so. Hashcash took a fair amount of computing power but it was very easy to verify. The verification would be performed by the user of course.

### 1998 b-money
In 1998 Wei Dai proposed b-money. It was the idea of creating money by solving cryptographic/computational puzzles like hashcash but based on a peer-to-peer network where every node maintained the list of transactions. 

### 2005 BitGold
In 2005 Nick Szabo (Who might be Satoshi) introduced BitGold by proposing on solving computational puzzles to “mint” digital cash and Hall Finney introduced a cryptographic currency by the idea of combining b-money and hashcash. Sadly enough it relied on a centralized authority. 

### 2009 Bitcoin
In 2009 a mysterious anonymous person shocked the world by creating the first practical implementation of digital cash/cryptocurrency called bitcoin. 
For the first time ever it managed to solve the problem of distributed consensus in a trustless network.

It uses pubkey cryptography together with hashcash as Proof Of Work to achieve a decentralized and secure method of minting/mining digital cash. The key of bitcoin was having an ordered list of blocks composed of transactions. 

Looking back it is now easier to see how combining all these concepts were combined to invent bitcoin and the blockchain.

Satoshi Nakamoto called his whitepaper "Bitcoin: A Peer-to-Peer Electronic Cash System" and his original whitepaper can be found here: https://bitcoin.org/bitcoin.pdf

Special thanks to @BTCYamakaza for editing