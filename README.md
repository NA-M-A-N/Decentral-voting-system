# Decentral-voting-system using ethereum blockchain 
The Decentralized Voting System using Ethereum Blockchain is a secure and transparent solution for conducting elections. Leveraging Ethereum's blockchain technology, this system ensures tamper-proof voting records, enabling users to cast their votes remotely while maintaining anonymity and preventing fraud. Explore this innovative project for trustworthy and decentralized voting processes.
# Features
* Implements JWT for secure voter authentication and authorization.
* Utilizes Ethereum blockchain for tamper-proof and transparent voting records.
* Removes the need for intermediaries, ensuring a trustless voting process.
* Admin panel to manage candidates, set voting dates, and monitor results.
* Intuitive UI for voters to cast votes and view candidate information.
# Requirements
* Node.js (version – 18.14.0)
* Metamask
* Python (version – 3.9)
* FastAPI
* MySQL Database (port – 3306)
# Installation

1. Open a terminal.

2. Clone the repository by using the command

3. git clone <pre lang=LANG> https://github.com/Krish-Depani/Decentralized-Voting-System-Using-Ethereum-Blockchain.git

4. Download and install Ganache.

5. Create a workspace named developement, in the truffle projects section add truffle-config.js by clicking ADD PROJECT button.

6. Download Metamask extension for the browser.

7. Now create wallet (if you don't have one), then import accounts from ganache.

8. Add network to the metamask. ( Network name - Localhost 7575, RPC URl - http://localhost:7545, Chain ID - 1337, Currency symbol - ETH)

9. Open MySQL and create database named voter_db. (DON'T USE XAMPP)

 10. In the database created, create new table named voters in the given format and add some values.

    CREATE TABLE voters (
    voter_id VARCHAR(36) PRIMARY KEY NOT NULL,
    role ENUM('admin', 'user') NOT NULL,
    password VARCHAR(255) NOT NULL
    );

   11. Install truffle globally

  
  12. Go to the root directory of repo and install node modules
13. Install python dependencies



# code structure 
<pre lang=LANG> ├── blockchain-voting-dapp            # Root directory of the project.
    ├── build                         # Directory containing compiled contract artifacts.
    |   └── contracts                 
    |       ├── Migrations.json       
    |       └── Voting.json           
    ├── contracts                     # Directory containing smart contract source code.
    |   ├── 2_deploy_contracts.js     
    |   ├── Migrations.sol            
    |   └── Voting.sol                
    ├── Database_API                  # API code for database communication.
    |   └── main.py                   
    ├── migrations                    # Ethereum contract deployment scripts.
    |   └── 1_initial_migration.js    
    ├── node_modules                  # Node.js modules and dependencies.
    ├── public                        # Public assets like favicon.
    |   └── favicon.ico               
    ├── src                           
    |   ├── assets                    # Project images.
    |   |   └── eth5.jpg              
    |   ├── css                       # CSS stylesheets.
    |   |   ├── admin.css             
    |   |   ├── index.css             
    |   |   └── login.css             
    |   ├── dist                      # Compiled JavaScript bundles.
    |   |   ├── app.bundle.js         
    |   |   └── login.bundle.js       
    |   ├── html                      # HTML templates.
    |   |   ├── admin.html            
    |   |   ├── index.html            
    |   |   └── login.html            
    |   └── js                        # JavaScript logic files.
    |       ├── app.js                
    |       └── login.js              
    ├── index.js                      # Main entry point for Node.js application.
    ├── package.json                  # Node.js package configuration.
    ├── package-lock.json             # Lockfile for package dependencies.
    ├── README.md                     # Project documentation.
    └── truffle-config.js                    # Truffle configuration file.
