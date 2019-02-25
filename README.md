## Install
```
$ go get github.com/etclabscore/devp2ping/...
```

## Help

```
$ devp2ping -h

    Spins up a memory-backed p2p server and attempts to make a very basic connection with an enode.

Usage:
  devp2ping <enode> [flags]

Flags:
  -h, --help          help for devp2ping
  -t, --timeout int   time in seconds to wait for node to dial a connection (default 30)
```

## Use

```
$ devp2ping enode://66498ac935f3f54d873de4719bf2d6d61e0c74dd173b547531325bcef331480f9bedece91099810971c8567eeb1ae9f6954b013c47c6dc51355bbbbae65a8c16@54.148.165.1:30303
```

Returns exit code `0` if successful, `1` if failed.

#### Check default go-ethereum/multi-geth bootnodes

If you have a `go-ethereum` source (eg. [ethoxy/multi-geth](https://github.com/ethoxy/multi-geth) or [ethereum/go-ethereum](https://github.com/ethereum/go-ethereum)) available in your $GOPATH, you can run checks for default bootnodes with

```
$ ./check-bootnodes.sh [<chain> ...]
```

