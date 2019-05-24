# Docker List Tags

Bash script for retrieving all version tags for any Docker image from the Docker registry.

## Usage

```
docker-list-tags <image name>
```

### Example

```
$ docker-list-tags mysql
Available tags for mysql

latest          5.5.47          5.5.57          5.6.22          5.6.32          5.6.42          5.7.16          5.7.26          5.7.8-rc        8.0.15
5               5.5.48          5.5.58          5.6.23          5.6.33          5.6.43          5.7.17          5.7.4           5.7.9           8.0.16
5.5             5.5.49          5.5.59          5.6.24          5.6.34          5.6.44          5.7.18          5.7.4-m14       8               8.0.2
5.5.40          5.5.50          5.5.60          5.6.25          5.6.35          5.7             5.7.19          5.7.5           8.0             8.0.3
5.5.41          5.5.51          5.5.61          5.6.26          5.6.36          5.7.10          5.7.20          5.7.5-m15       8.0.0           8.0.4
5.5.42          5.5.52          5.5.62          5.6.27          5.6.37          5.7.11          5.7.21          5.7.6           8.0.1           8.0.4-rc
5.5.43          5.5.53          5.6             5.6.28          5.6.38          5.7.12          5.7.22          5.7.6-m16       8.0.11
5.5.44          5.5.54          5.6.17          5.6.29          5.6.39          5.7.13          5.7.23          5.7.7           8.0.12
5.5.45          5.5.55          5.6.20          5.6.30          5.6.40          5.7.14          5.7.24          5.7.7-rc        8.0.13
5.5.46          5.5.56          5.6.21          5.6.31          5.6.41          5.7.15          5.7.25          5.7.8           8.0.14
```

## Requirements

The following two programs need to be installed on your system:

- [curl](https://curl.haxx.se/) for downloading the tag data from the Docker registry
- [jq](https://stedolan.github.io/jq/) for parsing the JSON response and extracting version numbers

### Debian & Ubuntu

```
sudo apt update && sudo apt install curl jq
```
