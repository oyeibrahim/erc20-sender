# ethereum-sender
Complete JS implementation of sending ERC20 token programmatically using Web3 and Infura.

You must have read and understand web3 Documentation on sending Ethereum transaction before using this code.
The documentation is available here: https://web3js.readthedocs.io/en/v1.3.0/web3-eth.html#sendtransaction

You MUST get an ETH provider API token, e.g Infura
Get infura token here https://infura.io/

The compulsory modules are:
web3 - for accessing Ethereum Blockchain
ethereumjs-tx - ethereum library for doing core ethereum tasks like signing transaction

Any other module is just for browser testing (express) or info hidding (dotenv)

The supported tokens must be saved in the /tokens folder. 
The token file must be in small letter
The data in the token file must include the token:
* Name
* Ticker
* ABI
* Address
* Decimal
* Decimal Rept : the representation of the token decimal in Ethereum Standard, check https://web3js.readthedocs.io/en/v1.2.11/web3-utils.html#towei

An example file is available in the folder.

It is not compulsory to introduce the token data in this form, you can choose any other form to get the token data. Sending ERC20 requires the token contract ABI, Address and Decimal. Those three must be introduced in any way before the transfer can work.
