# Blockchain in Python 

This project contains multiple pieces to create a functional of blockchain (although **not production ready**) 

It also suport wallet as an escrow and leverages the events triggered from the blockchain.


## overview of the project

- Blockchain.py file: This file is the main class used to define functions such as transaction, wallet, proof of work, mining hashing, nonce and generating the genesis.
- block.py file: This file is defined as the class of block synchronisation.
- Transcation.py file: This file is defined the class of transaction which can be added to a block in the blockchain.
- Wallet.py file: This file is defined the class of the wallet conception used to interact with the blockchain. Creates, loads and holds private and public keys. Manages transaction signing and verification.
- Node.py file: This file is the flask app class that combined the others class to run. 
- OLD-node.py file: This file is run two diffrent blockchain for synchronisation.
- ui file content the user interface for (network.html and node.html).
- Utility file, this file contents the support of the verfication and imporovment.

## Requirements

- python 3 and above
- pip install Flask
- pip install crypto
- pip install Flask-Cors

## Build & Compile

- Python3 node.py 
- Running on all addresses (0.0.0.0)
 * Running on http://127.0.0.1:5000  new node
 * Running on http://192.168.1.8:5000 old node

### Front-end

- UI , will run the flask on network.html by calling the class of the node.py.


### Back-end

- Node.py class will calling the class of the blockchain.py, old-node.py, Transcation.py, block.py and wallet.py.
