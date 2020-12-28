# Clusterizer

Walks the parsed blocks and clusterizes addresses based on [Common Input heuristic](http://127.0.0.1:3000/heuristics/heuristics.html#heuristics).

## Configuration

```
Clusterizer service in bitgodine architecture in charge of keeping
cluster of addresses up to date based on chain stored in local storage.

Usage:
  clusterizer [command]

Available Commands:
  export      Export stored clusters to csv
  help        Help about any command
  start       Creates clusters from synced blocks
  version     bitgodine-clusterizer version

Flags:
      --db string       Sets the path to the storage stored files (default "/badger")
      --debug           Sets logging level to Debug
  -h, --help            help for clusterizer
  -o, --output string   Sets the path to output clusters.csv file (default "/home/xn3cr0nx/.bitgodine")

Use "clusterizer [command] --help" for more information about a command.
```
