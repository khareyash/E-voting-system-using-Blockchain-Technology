# E-voting-system-using-Blockchain-Technology
A blockchain is designed to be accessed across a peer-to-peer network, each node/peer then
communicates with other nodes for block and transaction exchange. Once connected to the
network, peers start sending messages about other peers on the network, this creates a
decentralized method of peer discovery. The purpose of the nodes within the network is to
validate unconfirmed transactions and recently mined blocks, before a new node can start to do
this it first has to carry out an initial block download. The initial block download makes the new
node download and validate all blocks from block 1 to the most current blockchain, once this is
done the node is considered synchronized.
Blockchain instead of a centralized database, all the transaction data that is shared across the
nodes in the blockchain is contained in bundles of records called blocks, which are chained
together to create the public ledger. This public ledger represents all the data in the blockchain.
All the data in the public ledger is secured by cryptographic hashing and validated by a
consensus algorithm. Nodes on the network participate to ensure that all copies of the data
distributed across the network are the same. That’s one very important reason why we’re
building our voting application on the blockchain because we want to ensure that our vote was
counted and that it did not change.
A website is designed that will be connected to the backend blockchain smart contract. This
website will first authenticate and authorize the user. This is done by taking the information from
the user and then that given information will be checked by the information that is already stored
in the database which will be kept in a server. That server will be connected to our website by
PHP and once the voter inserts his/her information, it will check the authenticity of the voter and
only if the voter is eligible to vote i.e. his/her information is present in the database and have not
voted before only then the voter will be directed to a webpage from which he/she can vote. This
system will keep a check on the duplicacy of votes i.e. no two votes can be cast from one user
When the authorization will be completed the user will be directed to another webpage which
will show the options of the candidates participating in the election so that the user can choose
from among those and cast his/her votes.
The webpage which shows the list of candidates for the voter to vote is developed in HTML and
connected to a backend blockchain smart contract developed in solidity language. Once the voter
has casted the vote, the information will flow through the smart contract and the count of votes
of the selected candidate will get updated.
Solidity will be used to develop smart contracts as back-end language which will help us to
provide this functionality. This solidity program will take the ethers with the help of Ethereumjs-test rpc which provides us with a number of dummy accounts with some dummy ethers so that the code can be uploaded to the blockchain network. After this function, Web3js is injected which is used to interact with the smart contract that is developed on the remix ide with the HTML page that shows the information of the program and calls the function of setting the value of votes and also displaying the count of votes. This takes care of most of the non-functional requirements like security, reliability, and accountability. This smart contract will contain all the candidates and their vote counts in separate variables which will be getting updated during the
process of voting.
