# Spider

Crawler service that scrapes the web in order to extract new tags to identify address clusters

## Configuration

```
Spider service crawling many web resources to sync and update addresses tags storage

Usage:
  spider [command]

Available Commands:
  crawl       Crawl resources as cronjob
  help        Help about any command
  version     bitgodine-spider version

Flags:
      --cron            Sets if spider should be started as cron or just run once (default true)
      --debug           Sets logging level to Debug
  -h, --help            help for spider
      --target string   Sets if spider should run once with a specific target

Use "spider [command] --help" for more information about a command.
```
