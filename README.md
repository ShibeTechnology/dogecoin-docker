# Dogecoind docker container

```
$ docker build -t dogecoind .
$ docker run --rm --network=host -u $(id -u):$(id -g) --mount "type=bind,src=$(pwd)/data,dst=/mnt/data" -v $PWD/dogecoin.example.conf:/mnt/dogecoin.conf:ro dogecoind
```

## Notes

You should modify the `RPCUSER` and `RPCPASS` value.
