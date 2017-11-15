Raiden Network
==============

.. image:: https://badges.gitter.im/Join%20Chat.svg
    :target: https://gitter.im/raiden-network/raiden?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge
    :alt: Chat on Gitter

`Raiden Network documentation`_

.. _Raiden Network documentation: http://raiden-network.readthedocs.io/

The Raiden Network is an off-chain scaling solution, enabling near-instant, low-fee and scalable payments. It’s complementary to the Ethereum blockchain and works with any ERC20 compatible token.

The Raiden project is work in progress. Its goal is to research state channel technology, define protocols and develop reference implementations.

For more information please visit http://raiden.network/.

Installation
------------

Please refer to the `Installation`_ section in the official docs.

.. _Installation: http://raiden-network.readthedocs.io/en/stable/overview_and_guide.html#installation


Mike's Notes from Experience:

On Mac:

For installation:


You will run into 2 issues on mac:

1. You will be missing libcrypto: follow this: http://mithun.co/hacks/
library-not-loaded-libcrypto-1-0-0-dylib-issue-in-mac/ .... your version will be different but instruction works. But brew install openssl might be all you need.

2. You will be missing libgmp after pip install when running raiden, so do this:

brew update && brew install gmp
And you should be good to run

3. Solidity compiler: on mac:  brew tap ethereum/ethereum

Then: brew install solc


to run:
1. virtualenv raiden_project
2. source raiden_project/bin/activate

Have your Ethereum wallet set up, with your account, you will choose from there
On first go, it will ask for a file, you can generate a keystore on myetherwallet, put the JSON in a folder and unlick, but it will set go with your geth
Have geth running, and macke sure to "geth attach" and run getLatestBlock or what not to ensure you're synced
Then, all this other code should work



Ethereum mainnet
---------------

These are the currently deployed raiden contract addresses for the Ropsten testnet:

* Netting Channel Library: 0x7ce1cef50c3c72952e851af7e6787d7d19a740e9_
* Channel Manager Library: 0x51191c7d6d35e45909051035b79e09f7ba14c93a_
* Registry Contract: 0x93a89Beb5fc1539D5366382F8FEC1C774a572c84_
* Discovery Contract: 0x12a01d97c7976a08504bdcef1afdd5daf8e20d97_


Ropsten testnet
---------------

These are the currently deployed raiden contract addresses for the Ropsten testnet:

* Netting Channel Library: 0xad5cb8fa8813f3106f3ab216176b6457ab08eb75_
* Channel Manager Library: 0xdb3a4dbae2b761ed2751f867ce197c531911382a_
* Registry Contract: 0x68e1b6ed7d2670e2211a585d68acfa8b60ccb828_
* Discovery Contract: 0x1e3941d8c05fffa7466216480209240cc26ea577_




.. _0xad5cb8fa8813f3106f3ab216176b6457ab08eb75: https://ropsten.etherscan.io/address/0xad5cb8fa8813f3106f3ab216176b6457ab08eb75#code
.. _0xdb3a4dbae2b761ed2751f867ce197c531911382a: https://ropsten.etherscan.io/address/0xdb3a4dbae2b761ed2751f867ce197c531911382a#code
.. _0x68e1b6ed7d2670e2211a585d68acfa8b60ccb828: https://ropsten.etherscan.io/address/0x68e1b6ed7d2670e2211a585d68acfa8b60ccb828#code
.. _0x1e3941d8c05fffa7466216480209240cc26ea577: https://ropsten.etherscan.io/address/0x1e3941d8c05fffa7466216480209240cc26ea577#code
