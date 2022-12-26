# Robust Boilerplate for Hardhat Deployments

This is a boilerplate for quick contract development; meaning that getting started is as simple as using `yarn diag` to autogenerate a `.env` file. From here, your environment is immediately ready for use on `polygon`, `mumbai`, `goerli`, `ethereum`, `bsc`, `bscTestnet`, `opera`, `ftmTestnet`, `avax`, & `fuji`. To see the autogenerated config, simply run the `diag` script again!

## Video

[![Video Walkthrough](https://github.com/HemlockStreet/automated-hardhat-boilerplate/blob/main/thumbnail.png)](https://drive.google.com/file/d/1jPSUy3SLFO-ZamNfwEIoAkS_iYw41Di3/view?usp=share_link)

## Features

Credentials:

- .env autogeneration triggered just by using `npx hardhat`
- if no wallets are found, it will randomly generate 5 wallets and store them in your .env file
- .env diagnostics with `require('./utils/evm/diagnostics.js')` or `yarn diag`

Settings:

- preconfigured gas reporter (NOTE: disabled until you provide your own API key)
- preconfigured networks with free rpc providers

Deployments:

- deployment scripts with built-in contract auto-verification. (NOTE: disabled until you provide your own API key)
- all deployed contract ABIs are stored in `./utils/interfaces`
- all deployed contract addresses are stored in `./utils/deploymentMap/${chainId}.json` organized by contract name.

## API Keys

and where to find them...

- [COINMARKETCAP_API_KEY](https://pro.coinmarketcap.com/)
- [ETHERSCAN](https://etherscan.io/)
- [POLYGONSCAN](https://polygonscan.com/)
- [BSCSCAN](https://bscscan.com/)
- [FTMSCAN](https://ftmscan.com/)
- [SNOWTRACE](https://snowtrace.io/)