# EpicChain MetaMask Snap

## Overview

The **EpicChain MetaMask Snap** represents a significant advancement in integrating blockchain technology with mainstream digital wallet solutions. This Snap provides MetaMask users with a direct and secure method to interact with the EpicChain blockchain, enabling a range of functionalities that enhance the user experience and expand the capabilities of MetaMask. With this Snap, users can seamlessly manage EpicChain assets, perform transactions, and engage with smart contracts—all from within the familiar MetaMask interface.

EpicChain, known for its robust and scalable blockchain solutions, has created this Snap to bridge the gap between its advanced blockchain infrastructure and the widespread adoption of MetaMask as a digital wallet. This integration not only simplifies the process of accessing EpicChain’s features but also enhances security and usability for everyday blockchain interactions.

## Usage

**Important:** The EpicChain MetaMask Snap is currently in beta, which means it relies on [MetaMask Flask](https://metamask.io/flask/)—a special version of MetaMask designed for experimental and development purposes. During this beta phase, it is crucial to ensure that no other versions of MetaMask are installed on your browser. Conflicting versions could interfere with the Snap’s functionality and lead to unexpected issues. For optimal performance, disable MetaMask and any other wallets that might override the `window.ethereum` object.

To begin using the EpicChain MetaMask Snap, you need to install it through the dedicated installation portal. You can do this by visiting [EpicChain Snap Installation](https://vitalwallet.xyz/). This portal provides an easy and straightforward process for adding the Snap to your MetaMask setup.

**Documentation:** Detailed user guides, FAQs, and troubleshooting information will be available soon. Stay tuned for comprehensive documentation that will assist you in fully utilizing the EpicChain MetaMask Snap.

## Development

### Prerequisites

To develop or contribute to the EpicChain MetaMask Snap, you must have [MetaMask Flask](https://metamask.io/flask/) installed. It is essential to have MetaMask Flask installed as no other versions of MetaMask should be present on your system to prevent any conflicts. MetaMask Flask is designed specifically for development and experimental purposes, ensuring that you have access to the latest features and updates for the Snap.

### Installation

Start by installing the necessary dependencies to set up your development environment. Execute the following command to install all required packages:

```bash
yarn
```

### Running the Snap

#### Build Wallet Adapter

To build the wallet adapter needed for development purposes, use the following command:

```bash
yarn workspace epicchain-snap-wallet-adapter build:dev
```

This command prepares the wallet adapter for integration with MetaMask, enabling the necessary functionality for interacting with the EpicChain blockchain.

#### Start Snap Development Server

To initiate the Snap development server, run:

```bash
yarn workspace epicchain-snap start
```

This command will start the Snap development server, which will be available at:

- Snap Server: [http://localhost:8080/](http://localhost:8080/)

This server hosts the Snap’s backend services and provides an environment for testing and debugging.

#### Develop the Dapp Site

For developing the decentralized application (Dapp) site that interacts with the EpicChain Snap, use:

```bash
yarn workspace wallet-site dev
```

This will start the development server for the Dapp site, accessible at:

- Dapp Site: [http://localhost:8000/](http://localhost:8000/)

The Dapp site provides a user interface for interacting with the Snap, allowing you to test its features and functionalities in a live environment.

## Deploy Wallet Site

When you are ready to deploy the EpicChain wallet site for production, follow these steps:

```bash
yarn

yarn workspace epicchain-snap-wallet-adapter build

yarn workspace wallet-site build
yarn workspace wallet-site start
```

This sequence of commands will build and deploy the production-ready versions of both the Snap and the Dapp site, making them available for general use.

## Support and Feedback

We value your feedback and are committed to improving the EpicChain MetaMask Snap. For any issues, feature requests, or general support, please visit the [EpicChain MetaMask Snap support page](https://github.com/epicchainlabs/epicchain-metamask-snap/issues). Here, you can report problems, suggest new features, and engage with the development community.

## Conclusion

The EpicChain MetaMask Snap is a powerful tool that integrates EpicChain’s blockchain capabilities with MetaMask’s user-friendly interface. By leveraging this Snap, MetaMask users can efficiently manage their EpicChain assets, execute transactions, and interact with smart contracts without leaving their digital wallet. This integration enhances both the functionality and accessibility of EpicChain’s blockchain solutions, making them more accessible to a broader audience.

As the EpicChain MetaMask Snap continues to evolve, we will provide updates and improvements to ensure a seamless and enriched user experience. We encourage you to explore its features, provide feedback, and stay engaged with the development process.
