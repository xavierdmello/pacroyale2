[![image](https://github.com/user-attachments/assets/f277b63a-75c8-4683-868a-db838788949d)](https://dorahacks.io/buidl/20381)

On-Chain Real-Time Pac-Man Battle Royale, Winner Takes All.

Built on [Starknet](https://www.starknet.io/)

More info: https://dorahacks.io/buidl/20381

# Getting Started
1. Install Scarb, Starkli, and Starknet Foundry: https://docs.starknet.io/quick-start/environment-setup/
2. Install Starknet Devnet: https://0xspaceshard.github.io/starknet-devnet-rs/
3. Run Starknet Devnet: `starknet-devnet --seed 0`
4. Build contracts:
      - `cd ./cario`
      - `scarb build`
5. Deploy contracts:
      - `starkli declare target/dev/hello_world_PacRoyale.contract_class.json --rpc http://127.0.0.1:5050 --account ../account0_account.json --keystore ../account0_keystore.json`
      - Take note of the outputted class hash and replace CLASS_HASH with it in the next step
      - `starkli deploy CLASS_HASH --rpc http://127.0.0.1:5050 --account ../account0_account.json --keystore ../account0_keystore.json`
6. `cd ../frontend/src/components/`
7. Enter PACROYALE_ADDRESS address into `ContractAddresses.tsx`
8. Install packages
       - `cd ../../`
       - `pnpm i`
9. Start app: `pnpm dev`
10. Head to the displayed url and play! ex. http://localhost:5173/ 
