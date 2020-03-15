=======================
Getting Started with Smart Contracts on Bitcoin
=======================

Jargon and Basics
-----------------

Know all about how Bitcoin works? Skip to Setting-Up_.

.. _setting-up:

The concepts are rather simple but obscure terms may confuse someone starting out or coming from another procotol.
Here we define the essential jargon:

UTXO
  - Unspent transaction(TX) Output.
  - Located at an address.
  - Can contain bitcoin.
  - Imagine it as an envelope that can be opened (unlocked) only once.
<hope to get a a screenshot of CSW's envelope description from Metanet ICU, but haven't found it yet>

Transaction
  - Contains a Smart Contract
  - Can create multiple UTXOs

Address
  - Unique identifier of a UTXO in the Bitcoin Blockchain
  - A Public Key

Wallet
  - Can own multiple UTXOs
  - During a Transaction it gathers enough bitcoin from its UTXOs to cover the cost of the Transaction
  
    - eg. A wallet sends 10 bitcoin to another wallet.  Say it owns two UTXOs, one containing 7 bitcoin and another containing 4, these two are unlocked.  The transaction creates two new UTXOs: one containing 10 bitcoin to be received by the other wallet and another containing the change of 1 bitcoin, still to be owned by the sending wallet.

Miner
  - Validates transactions.  
  - If a Transaction is valid the Miner executes it and adds the Transaction's UTXOs to the Bitcoin Blockchain.

Smart Contract
  - Executed by miners, if they confirm the Transaction is valid
  - Contained in a UTXO.
  - Contains a locking script to seal the envelope(UTXO) and an unlocking script to open it.
  - Written in a Forth-like low level language called Bitcoin Script
  - Can be used for a wide variety of purposes, some simple common examples:
  
    - to send bitcoin to a specified wallet
    - for a Miner to redeem their newly mined bitcoins
    - to require the approval of multiple individuals to execute a transaction

P2PKH
  - Stands for Pay to Public Key Hash.
  - The most common type of Smart Contract
  - Sends bitcoins to a single Address, identified by the recipient's Address' Public Key Hash.

sCrypt
  - A language and IDE for writing Smart Contracts for Bitcoin.
  - A high level language, similar to JavaScript, that compiles to Bitcoin Script.
  - Its name originated from a combination of 'script' and 'Ncrypt'(previous name of nChain).

Setting Up
----------
work in progress... will add vscode install, testnet setup ready to make the P2PKH 
then step by step through to publishing and testing

.. code-block:: solidity
    
    contract Test {
    }


text ``code()``

