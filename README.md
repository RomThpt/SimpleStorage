# SimpleStorage Smart Contract

A minimal Solidity smart contract that demonstrates how to store, retrieve, and map favorite numbers to names on the Ethereum blockchain. Perfect for getting started with Solidity and smart contract basics. This project is part of my learning journey in blockchain development, following a course by **Cyfrin Updraft**.

## 📖 Overview

The **SimpleStorage** contract allows you to:
1. **Store a favorite number**.
2. **Retrieve the stored number**.
3. **Add people** to a list along with their favorite number.
4. **Map** each person’s name to their favorite number for easy look-up.

## 🚀 Features
- store: Save a favorite number on the blockchain.
- retrieve: Retrieve the stored number.
- addPerson: Add a person’s name and favorite number to the list and map.
- Mapping: Quickly access a person’s favorite number using their name.

## 📦 Installation

To deploy and test this contract locally, follow these steps:

1. Clone the Repository

```git 
git clone https://github.com/yourusername/simplestorage.git
```
2.	Install Dependencies
    
Install forge, a development environment for Ethereum.

3.	Compile the Contract
```console
forge compile
```

4.	Deploy the Contract
```console
forge deploy script/DeploySimpleStorage.s.sol --rpc-url $YOUR_RPC_URL --account $YOUR_ACCOUNT --sender $ACCOUNT_ADDRESS_KEYSTORE --broadcast
```

## 🛠 Usage

### Using Remix

You can test the contract directly in Remix IDE:

1.	Copy the contract code.
2.	Paste it into a new file in Remix.
3.	Compile and deploy it on a test network.

Interacting with Functions

- **Store**: Save a favorite number by calling store(uint256).
- **Retrieve**: View the stored number with retrieve().
- **Add a Person**: Use addPerson(string name, uint256 favoriteNumber) to add a person to the list.

### 🧩 Example Usage

1.	Store a number:

```
store(42);
```
2.	Retrieve the stored number:

```
retrieve(); // Returns: 42
```
3.	Add a person with their favorite number:

```
addPerson("Alice", 10);
```
4.	Look up Alice’s favorite number:
```
nameToFavoriteNumber("Alice"); // Returns: 10
```


## 🤝 Contributing

1.	Fork the repository.
2.	Create a new branch for your feature (git checkout -b feature/YourFeature).
3.	Commit your changes (git commit -m 'Add YourFeature').
4.	Push to the branch (git push origin feature/YourFeature).
5.	Open a Pull Request.

### 📄 License

This project is licensed under the **MIT License** - see the LICENSE file for details.

----

### Happy coding! 🚀
