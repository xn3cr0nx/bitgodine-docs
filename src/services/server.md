# Server

REST API the expose multiple endpoints to interact with the bitgodine system. The complete endpoint swagger documentation is available at [swagger.bitgodine.com](https://swagger.bitgodine.com).

## Configuration

```txt
Go implementation of Bitcoin forensic analysis tool to investigate blockchain and Bitcoin malicious flows.

Usage:
  bitgodine [command]

Available Commands:
  help        Help about any command
  serve       Serve bitgodine web server
  version     bitgodine-server version

Flags:
      --analysis string       Sets the path to the analysis stored files (default "/analysis")
      --badger string         Sets the path to the badger stored files (default "/badger")
      --bitgodineDir string   Sets the folder containing configuration files and stored data (default "/home/xn3cr0nx/.bitgodine")
  -b, --blocksDir string      Sets the path to the bitcoind blocks directory (default "/home/xn3cr0nx")
      --dbDir string          Sets the path to the indexing db files (default "/home/xn3cr0nx/.bitgodine/badger")
      --debug                 Sets logging level to Debug
  -h, --help                  help for bitgodine

Use "bitgodine [command] --help" for more information about a command.
```
