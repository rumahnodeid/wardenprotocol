![Warden Protocol](./docs/logo.svg)

Monorepo for Warden Protocol and its services.

More general information about the project can be found at:
https://wardenprotocol.org/.

If you want to learn more, join the network or contribute to the code, check
out the documentation website at: https://docs.wardenprotocol.org/.


## License

## RUNNING WARDEN-PROTOCOL TESTNET
## SPESIFICATION REQUIREMENT AND RUNNING ON MY OWN SERVER 
8 Cores, 16GB RAM DDR4,  512G SSD, Ubuntu 22.04

## JOINING ALFAMA TESTNET
```git clone --depth 1 --branch v0.1.0 https://github.com/warden-protocol/wardenprotocol/
cd  wardenprotocol/warden/cmd/wardend
go build

sudo mv wardend /usr/local/bin/
wardend init <your-node-name>
```

Prepare genesis file

```
cd $HOME/.warden/config
rm genesis.json
wget https://raw.githubusercontent.com/warden-protocol/networks/main/testnet-alfama/genesis.json

# Set minimum gas price & peers
sed -i 's/minimum-gas-prices = ""/minimum-gas-prices = "0.0025uward"/' app.toml
sed -i 's/persistent_peers = ""/persistent_peers = "2fa750223e22cc19a96391be254680e76387039c@174.138.6.105:26656,12caf2f5e3618cb6c57f45e93ac713b2bc6243b1@164.90.205.67:26656,b9c77f2a0b725fb9b48b50e5ec50d100c58514af@165.232.87.163:26656"/' config.toml
```
## START THE NODE
```
wardend start
```
With the exception of the SpaceWard folder, this project is released under the
terms of the Apache 2.0 License - see [LICENSE](./LICENSE) for details.

Elements of this project are based on the work made by Qredo Ltd on [Fusion
Chain](https://github.com/qredo/fusionchain) and were released under the Apache
2 license. See [NOTICE](./NOTICE) for more details.

