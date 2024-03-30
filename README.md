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
git clone --depth 1 --branch v0.1.0 https://github.com/warden-protocol/wardenprotocol/
cd  wardenprotocol/warden/cmd/wardend
go build

sudo mv wardend /usr/local/bin/
wardend init <your moniker name>

With the exception of the SpaceWard folder, this project is released under the
terms of the Apache 2.0 License - see [LICENSE](./LICENSE) for details.

Elements of this project are based on the work made by Qredo Ltd on [Fusion
Chain](https://github.com/qredo/fusionchain) and were released under the Apache
2 license. See [NOTICE](./NOTICE) for more details.

