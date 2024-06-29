# Dkeeper-App

Welcome to my new dkeeper project and to the Internet Computer development. This project is a decentralized note-keeping application that leverages the power of the Internet Computer to securely store and manage notes in a decentralized manner.

## Table of Contents
- [Project Description](#project-description)
- [Technologies Used](#technologies-used)
- [How to Run](#how-to-run)
  - [Running the Project Locally](#running-the-project-locally)
  - [Development Server](#development-server)
- [Directory Structure](#directory-structure)
- [File Descriptions](#file-descriptions)
  - [`dfx.json`](#dfxjson)
  - [`src`](#src-folder)
- [Key Features](#key-features)
- [Contributions](#contributions)

## Project Description

Dkeeper is a decentralized note-keeping application built on the Internet Computer. Users can create, view, and delete notes. The notes are securely stored on the blockchain, ensuring immutability and decentralization.

## Technologies Used

- **Internet Computer**: Decentralized computing platform by DFINITY.
- **Motoko**: Programming language for developing on the Internet Computer.
- **React**: JavaScript library for building user interfaces.
- **dfx**: Command-line tool for managing Internet Computer projects.

## How to Run

### Running the Project Locally

To test your project locally, use the following commands:

```bash
rm -rf .dfx
```
 ### Removes the .dfx directory and all its contents, resetting the local state and requiring you to recompile and redeploy your canisters.

```bash
dfx start --background
```
#### Starts the replica, running in the background


```bash
dfx deploy
```
#### Deploys your canisters to the replica and generates your candid interface

Once the job completes, the application will be available at `http://localhost:8080?canisterId={asset_canister_id}`.

### Development Server
If you are making frontend changes, you can start a development server with:

```bash
npm start
```
This will start a server at `http://localhost:8080`, proxying API requests to the replica at port 8000.

# Directory structure

```bash
dkeeper
├── src
│   ├── dkeeper_assets
│   │   ├── src
│   │   │   ├── index.html
│   │   │   ├── index.js
│   │   │   └── ...
│   │   ├── dkeeper_assets
│   │   ├── declarations
│   │   └── ...
├── dfx.json
├── package.json
└── README.md
```

# File Descriptions
`dfx.json`
The configuration file for the dfx tool, specifying canister settings, network configurations, and other project-specific information.

`src` Folder
Contains the source code for the dkeeper application, including frontend assets and canister code.
- **`index.html`**: The main HTML file for the application.
- **`index.js`**: The main JavaScript file for the application.
- **Assets**: Static files (e.g., images, stylesheets).
- **Declarations**: Generated files that provide type information for interacting with canisters.

# Key Features
- **Create Notes**: Users can add new notes.
- **View Notes**: Users can view all their notes.
- **Delete Notes**: Users can delete notes.
- **Decentralized Storage**: Notes are stored on a blockchain.


# Contributions
If you would like to contribute to this project, please fork the repository and submit a pull request. For major changes, please open an issue first to discuss what you would like to change.
