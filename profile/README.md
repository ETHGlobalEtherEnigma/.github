# EtherEnigma

## Unlock Mysteries. Win Rewards. On the Blockchain.

### Introduction

**EtherEnigma** is a decentralized, blockchain-based riddle-solving game that brings the thrill of puzzles to the Ethereum ecosystem. Players stake Ether to participate, solve engaging riddles set by an AI agent, and stand a chance to win a share of the accumulating prize pool. The game leverages smart contracts to ensure fairness, transparency, and trustlessness.

### Motivation

In the rapidly evolving world of decentralized applications, combining entertainment with blockchain technology opens up new avenues for interactive and rewarding experiences. EtherEnigma aims to showcase how smart contracts can be used to create a fun, engaging game that also demonstrates the potential of decentralized finance and blockchain transparency.

### Features

- **Decentralized Gameplay**: All game logic is executed through Ethereum smart contracts, eliminating the need for a centralized authority.
- **Accumulating Prize Pool**: The prize pool grows with each player's stake and external contributions, increasing the potential rewards.
- **Challenging Riddles**: Players face intriguing riddles curated by an AI agent, adding an intellectual challenge to the game.
- **Fair and Transparent**: Smart contracts ensure that the game rules are enforced consistently and transparently.
- **Open for Contributions**: Anyone can contribute to the prize pool, and the contract owner can inject initial funds to kickstart the game.

### Coinbase Developer Platform (CDP) Integration

We built EtherEnigma using the **Coinbase Developer Platform (CDP)**, a suite of tools and services provided by Coinbase to simplify blockchain development.

#### What is CDP?

The Coinbase Developer Platform is designed to help developers build, test, and deploy decentralized applications (dApps) more efficiently. It offers:

- **Blockchain APIs**: Easy access to blockchain data and services.
- **Developer Tools**: Utilities for smart contract development, testing, and deployment.
- **Secure Infrastructure**: Reliable and secure endpoints for interacting with the blockchain.
- **Integration Support**: Seamless integration with Coinbase services and wallets.

By leveraging CDP, we were able to:

- **Accelerate Development**: Utilize ready-made APIs and tools to speed up the development process.
- **Ensure Security**: Benefit from Coinbase's secure infrastructure to protect our smart contracts and transactions.
- **Enhance User Experience**: Integrate with Coinbase Wallet to provide a smooth onboarding process for players.

For more information on CDP, visit the [Coinbase Developer Platform](https://developers.coinbase.com/).

### How It Works

1. **Stake to Play**: Players initiate the game by staking a predetermined amount of Ether.
2. **Riddle Assignment**: An authorized agent assigns a riddle to the player after they join.
3. **Attempt to Solve**: The player submits their answer within a specified time limit.
4. **Outcome**:
   - **Correct Answer**: The player wins half of the contract's current balance, while the remainder stays in the prize pool for future players.
   - **Incorrect Answer or Timeout**: The prize pool remains untouched, increasing the potential winnings for subsequent players.

### Technology Stack

- **Solidity**: Programming language for writing smart contracts.
- **Foundry**: A fast, portable toolkit for Ethereum application development.
- **Ethereum (Base Sepolia Testnet)**: Blockchain network for deploying and testing the smart contracts.
- **Coinbase Developer Platform**: Tools and infrastructure for blockchain development.
- **Web3 Libraries (Ethers.js/Web3.js)**: For interacting with the Ethereum network.

### Gameplay Instructions

1. **Player Participation**

   - **Start Game**: Players call the `startGame` function, sending the required stake amount.
   - **Wait for Riddle**: An agent assigns a riddle to the player.
   - **Submit Answer**: Players submit their answer using the `submitAnswer` function within the time limit.

2. **Agent Responsibilities**

   - **Monitor Events**: Listen for the `GameStarted` event to know when a player has joined.
   - **Assign Riddles**: Call `setRiddle` to assign a riddle and answer hash to the player.
   - **End Game if Necessary**: Use `endGame` to conclude a player's game if they exceed the time limit without submitting an answer.

### Contributing

We welcome contributions from the community!

- **Report Issues**: If you find bugs or have feature requests, please open an issue on GitHub.
- **Submit Pull Requests**: For code contributions, fork the repository and submit a pull request with your changes.
- **Join the Discussion**: Engage with us on GitHub Discussions to share ideas and collaborate.

### Future Improvements

- **Frontend Development**: Build a user-friendly interface for easier interaction.
- **Additional Riddles**: Integrate a broader set of riddles or allow community submissions.
- **Multiple Agents**: Support multiple agents to decentralize riddle assignments.
- **Enhanced Security**: Implement additional security measures like rate limiting and improved randomization.
- **Deeper CDP Integration**: Explore more features of the Coinbase Developer Platform to enhance functionality and security.

### License

This project is licensed under the [MIT License](LICENSE).

### Acknowledgments

- **Hackathon Organizers**: Thank you for providing the platform to develop and showcase this project.
- **Coinbase Developer Platform**: Special thanks to Coinbase for providing the tools and infrastructure that powered our development.
- **Community Contributors**: We appreciate everyone who has contributed to the project.

---

Enjoy unraveling the mysteries with **EtherEnigma**!

---

If you have any questions or need assistance, feel free to reach out through our GitHub repository.