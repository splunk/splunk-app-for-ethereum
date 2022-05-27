# Splunk App for Ethereum
The Splunk App for Ethereum provides a set of dashboards, macros and searches for Ethereum and Ethereum-based blockchain networks.  This app provides ledger analytics and node monitoring for any Ethereum-based (EVM) blockchain.  These dashboards are meant to be a starting point for building analytics around your environment whether your infrastructure is virtual or physical, on-premise or in the cloud.

The Splunk App for Ethereum is used in conjunction with [Splunk Connect for Ethereum](https://github.com/splunk/splunk-connect-for-ethereum) which provides the data ingestion for Ethereum-based blockchains. The dashboards in this app rely on a few pre-defined macros for index names.  Once you have successfully installed and configure Splunk Connect for Ethereum simply update name of the index in the [ethereum_index](https://github.com/splunk/splunk-app-for-ethereum/blob/master/default/macros.conf) macro and you're on your way.  You'll also notice that this app contains macros for parsing ERC20 tokens and few other goodies as well ;).  

## App Features

### Dashboards
There are several dashboards provided to get you started with analyzing Ethereum data. These include:

  * **[Introduction](./screenshots/Introduction.png)** - A dashboard to ensure that your Splunk environment is receiving data with links to other dashboards.
  * **[Ethereum Starter Searches](./screenshots/Starter_Searches.png)** - See at a glance the number of blocks, transactions, average block timings, distinct Eth Addresses and total Eth transferred (with built in links to Etherscan.io).
  * **[Multichain Stats](./screenshots/Multichain_Stats.png)** - Are you ingesting mainnet and other networks like Rinkeby or xDai?   Here you can see them all at a glance.   Cross Chain Analysis anyone?
  * **[Gas Analytics](./screenshots/GasAnalytics.png)** - Real time visibility into the fees being charged to execute transactions on Ethereum. This dashboard also includes a little ML to predict where gas prices will go in the future based on past history!
  * **[Explorers Galore](./screenshots/Eth_Address_Explorer.png)** - There are Explorer dashboards for raw blockchain data, Smart Contracts, Ethereum Addresses, Wrapped xDai, and NFT's!   
  * **[ABI Decoding](./screenshots/ABI_Decoding.png)** - That's right, Splunk can decode your Smart Contracts and show you all the transaction and transaction log events.
  * **[Node Monitoring](./screenshots/NNode_Health_SC4Eth.png)** - Whether you monitor your nodes with Splunk Infrastructure Monitoring, OpenTelemetry or Prometheus we have dashboards for the most common configurations.   We've even baked in the ability to link directly back to Splunk Observability Cloud for any specific instance.  

### Macros
The app provides a number of macros to make things easier.  There are macros for indexx names to make it easy for you to customize your environment, a macro to parse ERC-20 transactions and a few more to make trait parsing easier for NFTs.  

Please visit the [screenshots](./screenshots) directory or for more information visit our [documentation](https://www.splunkdlt.com/fabric/splunk-app-for-fabric).


# Getting Started

1. Install the App on a Splunk Enterprise Search Head that will have access to the data.  
2. Edit the Splunk Macro name `ethereum_index` and set the index name to whatever your ethereum index is.
3. Open the App and navigate to the “Introduction” dashboard.
*You are now ready to use the Splunk App for Ethereum!*

# License

Copyright 2021 Splunk Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.



## Support 💪
Please use the [GitHub Issue Tracker](https://github.com/splunk/splunk-app-for-ethereum/issues) to submit bugs or request features.  If you have a question, email us at [blockchain@splunk.com](mailto:blockchain@splunk.com)



## License
Copyright 2022 Splunk Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
