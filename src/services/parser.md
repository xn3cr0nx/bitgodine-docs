# Parser

Parser service parses the blockchain raw data files and extracts blocks in a convenient format.

## Configuration

```
Go implementation of Bitcoin forensic analysis tool to	investigate blockchain and Bitcoin malicious flows.

Usage:
  parser [command]

Available Commands:
  help        Help about any command
  start       Parses the blockchain to sync it
  version     bitgodine-parser version

Flags:
      --bitgodineDir string   Sets the folder containing configuration files and stored data (default "/home/xn3cr0nx/.bitgodine")
  -b, --blocksDir string      Sets the path to the bitcoind blocks directory (default "/home/xn3cr0nx")
      --btcCerts string       Specify bitcoin client connection certificates (default "~/.bitcoin/rpc.cert")
      --btcEp string          Specify bitcoin client endpoint protocol (default "ws")
      --btcHost string        Specify bitcoin client host (default "localhost:8333")
      --btcPass string        Specify bitcoin client connection password (default "pass")
      --btcUser string        Specify bitcoin client connection user (default "bitcoinrpc")
      --config string         config file (default is $HOME/.bitgodine.yaml)
      --db string             Sets the path to the indexing db files (default "/home/xn3cr0nx/.bitgodine/badger")
      --dbDir string          Sets the path to the indexing db files (default "/home/xn3cr0nx/.bitgodine/badger/skipped")
      --debug                 Sets logging level to Debug
      --file int              Sets the data file to start parsing from
  -h, --help                  help for parser
  -n, --network string        Specify blockchain network - mainnet - testnet3 - regtest [default: mainnet] (default "mainnet")
  -r, --realtime              Specify whether real time parsing is performed (client connection) (default true)
      --restored int          Sets the number of blocks to restore before the current synced height (default 50000)

Use "parser [command] --help" for more information about a command.
```