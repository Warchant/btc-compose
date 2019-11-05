# btc-compose

##### start nodes

```
docker-compose up -d
```

Go to http://localhost:3002

Bitcoin dir is mounted at [./config/btc](./config/btc).

**WARNING**: do not remove bitcoin.conf

##### see logs

```
docker-compose logs -f
```

##### remove containers

```
docker-compose down
```

##### cleanup blocks

```
git clean -fdx
```
This removes all unchecked data from git repo.

#### use bitcoin-cli

```
docker-compose exec btcd bitcoin-cli <any cli options>
```

##### generate 2 blocks

```
docker-compose exec btcd bitcoin-cli generate 2
```
