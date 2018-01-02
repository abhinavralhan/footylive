# footylive
> Command line interface for Hackers who love football ⚽

## Installation

**Run**

```shell
$ npm install -g footballcli
```

## How to get API Key?

Please register on [football-data.org](http://api.football-data.org/register) to get your API Key. Then run `$ sudo football config` to add your API Key. Requests made using API key increases your rate limit from 50 requests per day to 50 requests per minute.

## Usage

### Commands available

```shell
football <command>

Commands:
  scores     Get scores of past and live fixtures
  fixtures   Get upcoming and past fixtures of a league and team
  standings  Get standings of particular league
  lists      List of codes of various competitions
  config     Change configuration and defaults

Options:
  -h, --help  Show help                                          [boolean]
  
```

#### Command `scores`
Get scores of past and live fixtures


```shell
Usage: football scores [options]

Options:
  -h, --help  Show help                                          [boolean]
  -l, --live  Live scores                                        [boolean]
  -t, --team  Select team                                        [string]

Examples:
  football scores -t "Manchester United" -l
  
```

#### Command `fixtures`
Get upcoming and past fixtures of a league and team

```shell
Usage: football fixtures [options]

Options:
  -h, --help    Show help                                         [boolean]
  -t, --team    Team name or substring of it                      [string]
  -l, --league  League
  -n, --next    Next or upcoming matches                          [boolean]

Examples:
  football fixtures -l PL -d 5 -t "Manchester United" -n

```


#### Command `standings`
Get standings of particular league

```shell
Usage: football standings [options]

Options:
  -h, --help    Show help                                         [boolean]
  -l, --league  League to be searched                             [required]

Examples:
  football standings -l PL

```

#### Command `lists`
List of codes of various competitions

```shell
Usage: sudo football lists [options]

Options:
  -h, --help     Show help                                        [boolean]
  -r, --refresh  Refresh league ids                               [boolean]

Examples:
  sudo football lists -r

```

#### Command `config`
Change configuration and defaults

```shell
Usage: sudo football config

Options:
  -h, --help  Show help                                           [boolean]

Examples:
  sudo football config
  
```


## Related
You may find similar packages [here](http://api.football-data.org/libraries)

## License

[MIT](https://github.com/abhinavralhan/footylive/blob/master/LICENSE)
