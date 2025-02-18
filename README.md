# cardano-test

# Setup

## Prerequires
- k8s cluster (minikube)
- tool: kubectl

# Note
- download config (preprod testnet) into folder configs 

## Core node
- Issue: need delete db folder before run mithril bootstrap

## Sync db
- Issue: need download schema (use initContainer download before run sync-db); disable insert ledger (file db-sync-config)
