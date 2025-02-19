# cardano-test

# Setup

## Prerequires
- k8s cluster (minikube)
- tool: kubectl

## Run
- Start cluster: minikube start
- Install apps: cd manifests => kubectl kustomize | kubectl apply -f -

# Note
- download config (preprod testnet) into folder configs 

## Core node
- Issue: need delete db folder before run mithril bootstrap

## Sync db
- Issue: need download schema (use initContainer download before run sync-db); disable insert ledger (file db-sync-config)

# Documents
## Relay node
- Doc: https://developers.cardano.org/docs/operate-a-stake-pool/cardano-relay-configuration

## Block producer node
- Doc: https://developers.cardano.org/docs/operate-a-stake-pool/generating-wallet-keys


# TODO
- Make topology work, test when scale relay node (need enable metric-server)
- Setup monitor with prometheus and grafana: https://developers.cardano.org/docs/operate-a-stake-pool/grafana-dashboard-tutorial
- Config core node, test wallet, register stake address, register pool
- Test transactions ...

