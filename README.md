# avax1
Below is a guide to deploying an EVM subnet using the Avalanche CLI, adding the subnet to Metamask, connecting Remix to Metamask, deploying smart contracts, and testing the application.

### Deploying EVM Subnet with Avalanche CLI

1. **Install Avalanche CLI**: Follow the instructions [here](https://docs.avax.network/build/tutorials/platform-deployment/setting-up-avalanche-cli) to install the Avalanche CLI.

2. **Initialize Avalanche**: Initialize Avalanche using the command:
   ```bash
   avalancheGo init --network-id=5
   ```

3. **Start Node**: Start a node on the EVM subnet with the command:
   ```bash
   avalancheGo run --network-id=5 --staking-tls-enabled=false --staking-enabled=false --snow-sample-size=1 --snow-quorum-size=1
   ```

### Adding Subnet to Metamask

1. Open Metamask and click on the network dropdown.
2. Select "Custom RPC" and enter the details of your EVM subnet:
   - Network Name: Avalanche EVM
   - RPC URL: http://localhost:9650/ext/bc/C/rpc
   - Chain ID: 5
   - Symbol: AVAX
   - Block Explorer URL: [Leave blank or add if available]

### Connecting Remix to Metamask

1. Open Remix and navigate to the "Settings" tab.
2. Under "Plugin", select "Solidity Compiler".
3. Scroll down and select "Environment" > "Injected Web3".
4. Remix should automatically connect to Metamask.

### Deploying Smart Contracts

1. Write your smart contracts in the Remix IDE.
2. Compile the contracts by clicking on the "Compile" tab.
3. In the "Deploy & Run Transactions" tab, select the contract you want to deploy from the dropdown.
4. Choose the desired account from Metamask and click "Deploy".

### Testing Application

1. Once deployed, interact with your contracts using the Remix interface.
2. Deploy tokens, pools, or any other functionality provided by your contracts.
3. Test different functions and scenarios to ensure everything works as expected.

#### Project Overview
This project demonstrates how to deploy an EVM subnet using the Avalanche CLI, connect it to Metamask, and deploy and test smart contracts using Remix.

#### Instructions
1. **Deploy EVM Subnet**: Use the Avalanche CLI to deploy an EVM subnet.
2. **Add Subnet to Metamask**: Add the subnet to Metamask as a custom RPC network.
3. **Connect Remix to Metamask**: Connect Remix to Metamask using the Injected Web3 provider.
4. **Deploy Smart Contracts**: Write, compile, and deploy smart contracts using Remix.
5. **Test Application**: Interact with deployed contracts in Remix to test functionality.

#### Notes
- Ensure Avalanche CLI, Metamask, and Remix are properly configured and running.
- Modify RPC URL and network details according to your deployment setup.
- Use proper caution when deploying and testing smart contracts in a live environment.

By following these steps and guidelines, you can successfully deploy and interact with smart contracts on an EVM subnet using Avalanche, Metamask, and Remix.
