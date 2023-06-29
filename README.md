# Flow-Beginner-final-project

## Introduction
The CryptoPoops project is a smart contract written in Solidity that implements a Non-Fungible Token (NFT) collection. The project allows users to create, deposit, withdraw, and borrow NFTs. It also includes an interface for interacting with the NFT collection. This README.md file provides an overview of the project and its functionality.

## Project Structure
The CryptoPoops project consists of the following files:

CryptoPoops.cdc: This file contains the main smart contract code. It defines the CryptoPoops contract, which extends the NonFungibleToken contract and implements the NFT collection functionality.
Minter: This file defines the Minter resource, which is responsible for creating new NFTs.
## Smart Contract Explanation
The CryptoPoops contract is the main contract in the CryptoPoops project. It extends the NonFungibleToken contract, which provides basic functionality for managing NFTs. The CryptoPoops contract adds additional functionality specific to the CryptoPoops project.

The CryptoPoops contract includes the following main components:

totalSupply: A variable that keeps track of the total number of NFTs in the collection.
event declarations: These declarations define events that are emitted when certain actions occur, such as contract initialization, NFT withdrawals, and NFT deposits.
NFT resource: This resource represents an individual NFT. It includes properties such as id, name, favouriteFood, and luckyNumber. The init function is used to initialize the NFT with these properties.
CryptoPoopsNFTCollectionPublic interface: This interface defines functions for depositing NFTs, getting NFT IDs, and borrowing NFTs. The borrowAuthNFT function also includes a post condition to ensure that the borrowed NFT has the correct ID.
Collection resource: This resource represents the NFT collection. It implements the NonFungibleToken.Provider, NonFungibleToken.Receiver, NonFungibleToken.CollectionPublic, and CryptoPoopsNFTCollectionPublic interfaces. It includes functions for withdrawing, depositing, getting IDs, and borrowing NFTs.
createEmptyCollection function: This function creates a new empty NFT collection.
Minter resource: This resource is responsible for creating new NFTs. It includes a createNFT function that takes parameters for name, favouriteFood, and luckyNumber and returns a new NFT.

## Conclusion
The code is implementing a smart contract for managing and interacting with non-fungible tokens. It extends the NonFungibleToken contract and provides functions for depositing, withdrawing, and borrowing tokens. It also includes functions for creating new tokens and collections. NFTs are unique digital tokens recorded on a blockchain that certify ownership and authenticity, typically representing digital files.

