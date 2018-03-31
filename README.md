# Crypto Mining

Basic docker container for crypto mining using cpuminer.

Fork of https://github.com/wernight/docker-cpuminer-multi

## Use it right now

### Run
worker is set in cpuminer root directory so to start it :
```
docker run cpuminer -a ALGO -o URL -u USERNAME yo1l/crypto-mining -p PASSWORD
```

### SWARM Service
```
docker service create --name miner yo1l/crypto-mining \
 cpuminer -a ALGO -o URL -u USERNAME - p PASSWORD
```

## DIY : Build
```
docker build -t NAME .
```

## References
 - Docker HUB : https://hub.docker.com/r/yo1l/crypto-mining/
 - CPU Miner Multi : https://github.com/tpruvot/cpuminer-multi.git
 - CPU Miner OPT : https://github.com/JayDDee/cpuminer-opt
