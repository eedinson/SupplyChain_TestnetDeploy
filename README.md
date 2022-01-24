<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">SupplyChain_TestnetDeploy</h3>

  <p align="center">
    Ethereum blockchain for supply chain tracking deployed on Ropsten Testnet
    <br />
    <a href="https://github.com/eedinson/SupplyChain_TestnetDeploy"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/eedinson/SupplyChain_TestnetDeploy">View Demo</a>
    ·
    <a href="https://github.com/eedinson/SupplyChain_TestnetDeploy/issues">Report Bug</a>
    ·
    <a href="https://github.com/eedinson/SupplyChain_TestnetDeploy/issues">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

![contractTxDetails][contractTxDetails]

There are many great README templates available on GitHub; however, I didn't find one that really suited my needs so I created this enhanced one. I want to create a README template so amazing that it'll be the last one you ever need -- I think this is it.

Here's why:
* Your time should be focused on creating something amazing. A project that solves a problem and helps others
* You shouldn't be doing the same tasks over and over like creating a README from scratch
* You should implement DRY principles to the rest of your life :smile:

Of course, no one template will serve all projects since your needs may be different. So I'll be adding more in the near future. You may also suggest changes by forking this repo and creating a pull request or opening an issue. Thanks to all the people have contributed to expanding this template!

Use the `BLANK_README.md` to get started.

<p align="right">(<a href="#top">back to top</a>)</p>



### Built With

This section list any major frameworks/libraries used to bootstrap the project.

* [Solidity](https://docs.soliditylang.org/en/v0.8.11/)
* [Remix](http://remix.ethereum.org/)
* [Ropsten Etherscan](https://ropsten.etherscan.io/)
* [Metamask](https://metamask.io/)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

This is an example of how to set up the project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites for Ubuntu 18.04.6 LTS

This is an example of how to list things you need to use the software and how to install them.

* nvm version 0.38.0
  ```sh
  curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
  ```
  
* node version 8.12.0
  ```sh
  sudo apt remove -y nodejs
  ```
  ```sh
  curl -sL https://deb.nodesource.com/setup_8.x | sudo -E bash -
  ```
  ```sh
  sudo apt-get install -y nodejs
  ```
  ```sh
  nvm install 8.12.0
  ```
  ```sh
  nvm use 8.12.0
  ```
  ```sh
  node -v
  ```
  --> v8.12.0
  ```sh
  npm -v
  ```
  --> 6.4.1
* npm version 6.4.1 (if not already installed)
  ```sh
  sudo npm install -g npm@6.4.1
  ```
* truffle
  ```sh
  sudo npm i -g truffle
  ```
* Ganache
  [Ganache](https://trufflesuite.com/ganache/)
  * Ganache-cli (for terminal interaction)
    ```sh
    sudo npm install -g ganache-cli
    ```

### Smart contract

_Below is a list of smart contract development procedures with specific information to consider.

1. Start programming the smart contract in Solidity with Remix [http://remix.ethereum.org/](http://remix.ethereum.org/)
2. Create a contract file
    AMChain.sol
3. Use specific pragma
   ```sh
   pragma solidity ^0.4.25;
   ```
4. Version of a deployable smart contract for Ropsten without helper functions (Build version) `SupplyChain_deployedRopstenBuild.sol`<br />
   Build contract address:
   ```sh
   0x2aeCF4dDb24BbDb8b48b6ee906c125E5573BBc9C
   ```
6. Version of a deployable smart contract for Ropsten with helper functions for testing (Test version) `SupplyChain_deployedRopsten>Test.sol`<br />
   Test contract address:
   ```sh
   0xdeC79E73f2955b4ec5e1b1b7Ca758088bf82631a
   ```

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

The use of the smart contract build version is explained in detail below. The following metamask account addresses are used as an example:<br />
Supplier:
   ```sh
   0xebdc7eAdBCc95aa5911A571cC589B0A42119D5dD
   ```
DeliveryCompany:
   ```sh
   0xA4084Fc2FeCBC4E20BaA2b5FA9Af3f5C72906536
   ```
Customer:
   ```sh
   0x5c6743508a15829E7bcb0484AFEfB07f88BA6Ce5
   ```

1. Use the final Solidity code with the correct pragma line in Remix [http://remix.ethereum.org/](http://remix.ethereum.org/)

![pragma][pragma]

2. Set the correct Solidity compiler settings

![compilerSettings][compilerSettings]

3. Set Meatamask as the environment provider and select an account for the Supplier

![setMetamaskAccount][setMetamaskAccount]

4. Deploy the smart contract via Metamask and create an order<br />
   Enter the order details for Title and Description<br />
   Select a second address in your Metamask account for the delivery company and a third account address for the customer<br />
   Click Transact and wait for the Metamask notification<br />
   Confirm the transaction in Metamask

![createOrder][createOrder]

5. Check that the order was created and verify the contract functionality<br />
   Wait for Metamask to confirm the transaction (check if the debug notification is green)<br />
   Check getOrder functionality and search for orders by index (if you only created one order, the index is 0)<br />
   Verify that you can see the information entered when creating the order, also verify and copy the transaction hash from the debug notification

![verifyTransaction][verifyTransaction]

6. Search for the smart contract in Ropsten Etherscan [https://ropsten.etherscan.io/](https://ropsten.etherscan.io/)

![etherscan][etherscan]

7. View the transaction details of the transaction hash and click on the contract address

![etherscanTxDetails][etherscanTxDetails]

8. View the contract details and the contract transactions

![contractTxDetails][contractTxDetails]

9. Read contract informations<br />
   From here you can read out all transaction information of the smart contract. All transaction information is transparent, publicly available and secured by decentralized storage, but transaction participants are anonymous due to the cryptographic principles of the blockchain.

![readContractInformations][readContractInformations]


_For further explanations on the use of the smart contract, please refer to the relevant publication [Paper](https://example.com)_

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [x] Develop a smart contract
- [x] Deploy and publish the smart contract
- [ ] Add Backend functionality
- [ ] Write tests for the smart contract
- [ ] Add Frontend functionality
    - [ ] optimize everything
    - [ ] add additional functions

See the [open issues](https://github.com/eedinson/SupplyChain_TestnetDeploy/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Erik Westphal - [@LinkedIn](https://linkedin.com/in/erik-westphal-706a35223) - erik.westphal@uni-rostock.de

Project Link: [https://github.com/eedinson/SupplyChain_TestnetDeploy](https://github.com/eedinson/SupplyChain_TestnetDeploy)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Choose an Open Source License](https://choosealicense.com)
* [GitHub othneildrew Best-README-Template ](https://github.com/othneildrew/Best-README-Template)
* [Alexander Pliskin - How To Create Supply Chain dApp For Order Accounting](https://www.youtube.com/watch?v=lXWlJIvGRMk&list=PLQbzkJk10-f5jfVIhDh9QLcbSEA8JiA_j&index=1)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/eedinson/SupplyChain_TestnetDeploy/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/eedinson/SupplyChain_TestnetDeploy/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/eedinson/SupplyChain_TestnetDeploy/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/eedinson/SupplyChain_TestnetDeploy/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/eedinson/SupplyChain_TestnetDeploy/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
[pragma]: images/pragma.png
[compilerSettings]: images/compilerSettings.png
[setMetamaskAccount]: images/setMetamaskAccount.png
[createOrder]: images/createOrder.png
[verifyTransaction]: images/verifyTransaction.png
[etherscan]: images/etherscan.png
[etherscanTxDetails]: images/etherscanTxDetails.png
[contractTxDetails]: images/contractTxDetails.png
[readContractInformations]: images/readContractInformations.png
