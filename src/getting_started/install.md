# Install

The system installation is both available through Docker (suggested) or can be installed locally. Local installation requires multiple dependencies due to the [services required](http://127.0.0.1:3000/services/services.html) for the system to work.

## Docker

You suggest to use the docker-compose file you can find in the main [bitgodine repository](https://github.com/xn3cr0nx/bitgodine) in order to easily bootstrap the entire system.

First clone the repository:

```bash
git clone https://github.com/xn3cr0nx/bitgodine.git
```

Then run docker-compose:

```bash
docker-compose up -d
```

This will build bitgodine services and run the entire system. If you want to run production ready services, including web server, you can use the production file:

```bash
docker-compose -f docker-compose.prod.yml up -d
```

## Locally

In the following we will link to tutorials or insert required commands to install all the dependencies. The guide is currently primarily based on Ubuntu.

### Bitcoin node

You can find multiple guides about installing a Bitcoin full node. Here we link the [official Bitcoin instructions](https://bitcoin.org/en/full-node#costs-and-warnings) that support multiple platform.

### Go

You can find the instructions to install Go in the [offical reference](https://golang.org/doc/install) with support for multiple platforms.

### Redis

Redis can be easily installed as service under Ubuntu with the following commands:

```bash
sudo apt install redis-server
```

```bash
sudo systemctl enable redis-server.service
```

Check redis is correctly installed with

```bash
redis-cli info
```

### Postgres

Postgres can be easily installed as service under Ubuntu with the following commands:

```bash
sudo apt install postgresql postgresql-contrib
```

Then you can access postgres in order to check it is correctly installed and running:

```bash
sudo -i -u postgres
```

```bash
psql
```


### Services

All bitgodine services can be installed using Go.

#### CLI

```bash
go get github.com/xn3cr0nx/bitgodine/cmd/cli
```

this will install the parser binary in your $GOPATH. Probably you want to rename the binary in order to have a less generic name in you PATH (and this can be done for all the other following services). You can rename the binary as follows:

```bash
mv $GOPATH/bin/parser $GOPATH/bin/bitgodine-cli
```

#### Parser

```bash
go get github.com/xn3cr0nx/bitgodine/cmd/parser
```

#### Clusterizer

```bash
go get github.com/xn3cr0nx/bitgodine/cmd/clusterizer
```

#### Server

```bash
go get github.com/xn3cr0nx/bitgodine/cmd/server
```

#### Spider

```bash
go get github.com/xn3cr0nx/bitgodine/cmd/spider
```
