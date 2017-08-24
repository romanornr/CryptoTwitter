# Distributed systems and Byzantine nodes

To understand blockchains, it's essential to understand distributed systems. 
This is because a blockchain is a distributed system or decentralized distributed system.

### What is a decentralized distributed system?

A centralized system is one where the state of your system and the program is stored on a single computer. 
For example, let’s say you download a pdf document your boss sent you. If your computer crashes and you don’t have a backup, you are out of luck.

Now let's say you stored the pdf document in Google drive or Dropbox, that’s great. You can download your pdf document on another computer because Google drive and dropbox are examples of cloud storage where your files get stored on multiple computers.
Anyways, this is great because using it makes it fault-tolerant, the state is divided over multiple servers/computers. If the google or dropbox servers fails, it’s probably replicated over their other machines.

However Decentralized systems are complex. It’s considered to be an advanced topic in computer science.  So Distributed systems are a computing paradigm which uses 2 or more to work with each other. 

A node can be defined as a single server/computer/player in a distributed system. All nodes should be able to to send and receive messages from each other. Nodes can also be faulty or malicious. Unexpected behavior of a node on the network is part of the Byzantine problem. 

In a distributed design is coordination between nodes and fault tolerance a challenge. If some nodes become faulty or their connection breaks, the distributed system should tolerate this and continue to work without an error to get the desired result (Think of when you run your Bitcoin Core wallet or any other altcoin core wallet). 

### Byzantine

How can you design a system that can survive the worse possibly failures in a system. 
Let's say a node in your system is a “traitor node”. That node sends 1 answer to one node and a total different answer to the other node and this can lead to a wrong answer that your distributed system is trying to perform. This could happen for example if a node generates a null response or ran out of memory or owned by an attacker/hacker example. That may lead to a Byzantine failure. 

Now Bitcoin is the perfect example, since your computer should not trust every other node/peer in the network. It would be pretty bad if 1 node has problems and takes down the entire bitcoin network. 

Another example is flight systems like in the boeing 777 and 787. A hardware failure might exhibit Byzantine like behaviors, they have build a byzantine fault tolerant flight control system into these aircrafts. 

### CAP Theorem

Distributed systems can not have Consistency, Availability And Partition tolerance simultaneously. 

- Consistency: ensures all nodes in a distributed system have the latest copy

- Availability: System is up, accessible and accepts incoming requests and responding without any failures and when required.

- Partition: If a group of nodes fails, the distributed system continue to operate correctly. 

A distributed system can not have all properties at the same time but Blockchain somehow can. 

Fault tolerance is achieved by the use of replication. Consistency is achieved by using consensus algorithms to ensure all nodes have the same data, this is also called state machine replication. Blockchain is a sort of method to achieve state machine replication. 

The Byzantine generals problem (https://en.wikipedia.org/wiki/Byzantine_fault_tolerance#Byzantine_Generals.27_Problem)
was solved in 1999 and in 2009 the first implementation was made together with Bitcoin where Pow (Proof Of Work) algorithm was developed as a mechanism to achieve consensus.  

Consensus is a process of agreement between distrusting nodes on a final state of data. To achieve consensus, different algorithms can be used. The concept of multiple nodes (example hundreds or  thousands of nodes) is known as a distributed consensus.  