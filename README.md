# goerli


1. make path as in the service file `mkdir -p /data/erigon/build/bin/`
2. copy the __erigon__ and __rpcdeamon__ in there
3. `cp goerli.service /etc/systemd/system/goerli.service`
4. `cp ropsten.service /etc/systemd/system/ropsten.service`
5. `sudo systemctl enable jsonrpc.service goerli.service`
6. `sudo systemctl status jsonrpc.service goerli.service`
7. look up the real-time log at `sudo journalctl -u goerli.service -f`
