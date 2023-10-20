# GiveCup Technical Documentation 👨‍💻

Welcome to the technical documentation of GiveCup. This document provides a deeper dive into our various repositories, highlighting the technological stack, the functionalities they serve, and their role in the GiveCup & MultiversX ecosystems.

## 1. [client](https://github.com/GiveCup/client) :iphone:

### Overview
The `client` repository houses our mobile application, which is our primary user interface. Developed using React Native and Expo, it provides a seamless experience across both Android and iOS platforms.

### Technical Stack
- **React Native**: Used for building our cross-platform mobile application.
- **react-native-xportal**: Facilitates the connection with xPortal and the MultiversX network.
- **Expo**: A framework and a platform to build and deploy React Native projects.
- **MultiversX**: Integrated for blockchain functionalities.
- **TypeScript**: Ensures type safety and improves code quality.

### Functionality
The client app offers a gamified donation experience. Users can navigate through a list of NGOs, donate, and track their contributions. The app communicates with our backend through the `api` repository to fetch data and perform actions on the blockchain.

## 2. [sc-dynamic-rs](https://github.com/GiveCup/sc-dynamic-rs) :sparkles:

### Overview
This repository is responsible for the dynamic NFTs on our platform. Built on the MultiversX blockchain and written in Rust, it enables the creation and customization of our unique NFTs.

### Technical Stack
- **Rust**: Uses the `mx-sdk-rs` framework to work with the MultiversX VM.
- **MultiversX**: Where the Smart Contracts are deployed and interacted with.
- **xSuite**

### Functionality
The smart contract facilitates the minting, customization, and trading of our dynamic NFTs. Each NFT represents a customizable cup that can be donated for its value to chosen NGOs.

## 3. [sc-donations-rs](https://github.com/GiveCup/sc-donations-rs) :heart:

### Overview
Central to our donation mechanism, this Rust-based smart contract on the MultiversX blockchain oversees direct donations and the quadratic funding mechanism.

### Technical Stack
- **Rust**: Uses the `mx-sdk-rs` framework to work with the MultiversX VM.
- **xSuite**: a full suite for efficiently developing high-quality MultiversX smart contracts.
- **MultiversX**: Where the Smart Contracts are deployed and interacted with.

### Structure
`simple-donations`: Facilitates a direct network for connecting users with organizations. Users can directly send EGLD to their desired causes and further earn rewards and benefits from our platform.

`quadratic-funding`: Implements a Quadratic Funding algorithmic method, in order to promote fair distribution of funds and incentivize a more democratic way to public goods funding.


For a quick and good explanation of Quadratic Funding, [watch this explanatory video](https://www.youtube.com/watch?v=HJljTtLnymE).

WIP.

### Functionality
Users can send funds directly to NGOs or participate in the quadratic funding mechanism to promote fairer distribution. It collaborates with the `client` app for transaction execution.

## 4. [genezio](https://github.com/GiveCup/genezio) :cloud:

### Overview
The `genezio` module represents our serverless operations. It ensures that our backend operations are efficient and scalable without the overhead of traditional server management.

### Technical Stack
- **Genezio**: A serverless framework to facilitate our backend processes.

### Functionality
This module helps scale our backend resources based on the demand. It interfaces with the `api` and smart contracts, handling serverless execution of various backend tasks.

*Currently WIP!

## 5. [api](https://github.com/GiveCup/api) :computer:

### Overview
Our `api` repository is the bridge between the frontend and the various backend operations. It's crafted using Express.js, ensuring a smooth communication channel.

### Technical Stack
- **Express.js**: A minimal and flexible Node.js web application framework.
- **Supabase**: Used for caching the blockchain and faster data availablity.

### Functionality
The API handles data requests from the `client` app, executes transactions, and communicates with the DB. It ensures data integrity, security, and efficiency in all our operations, as well as quicker data fetching


