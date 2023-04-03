# Deployment of Erigon (using Cloudmos)
copied from https://gist.github.com/leetdev/d671c850f9b036c5fe5765595a41c6a2

## Create or import wallet
- Install [Keplr browser extension](https://www.keplr.app/download)
- Create an account and/or import mnemonic
- Switch to Akash network

## Fund the wallet
- See this [docs page](https://docs.akash.network/tokens-and-wallets/funding) if you want to request some tokens for deployment purposes
- At least 5 AKT deposit is required for all deployment requests + some gas for transactions + 0.6 AKT Cloudmos deployment fee

## Deploy the node
Follow [this guide](https://docs.akash.network/guides/cloudmos-deploy) to deploy the node, except:
- Instead of selecting the Minecraft template, click on `Upload SDL`
- Open a `YAML` file with the following contents:
```YAML
version: "2.0"

services:
  erigon:
    image: renx81/erigon:v2.42.0
    args:
      - "--datadir=/root/.local/share/erigon"
      - "--private.api.addr=0.0.0.0:9090"
      - "--txpool.disable"
      - "--torrent.download.rate=100mb"
      - "--http.api=web3"
      - "--http.addr=0.0.0.0"
      - "--http.vhosts=*"
      - "--ws"
    expose:
      - port: 8545
        as: 80
        to:
          - global: true
    params:
      storage:
        data:
          mount: /root/.local/share/erigon

profiles:
  compute:
    erigon:
      resources:
        cpu:
          units: 2.0
        memory:
          size: 16Gi
        storage:
          - size: 2Gi
          - name: data
            size: 2.5Ti
            attributes:
              persistent: true
              class: beta3
  placement:
    dcloud:
      pricing:
        erigon:
          denom: uakt
          amount: 10000

deployment:
  erigon:
    dcloud:
      profile: erigon
      count: 1
```
- Proceed to step 5 in the guide

## Manage the deployment
- [Cloudmos deployment dashboard](https://deploy.cloudmos.io/deployments)
- [How to use](https://docs.akash.network/guides/cloudmos-deploy/manage-deployments)

## Notes
Akash network is still in early stages and as such, many hurdles had to be overcome in the process of getting the first deployment to work. Here's a couple of things that will likely improve in the future:
- Erigon's official docker image sets up an unprivileged user in the container, but the persistent storage on the Akash provider is likely mounted with a different UID. This is a feature of Docker, and in normal cases, UID/GID can be configured at build time. In this case, however, the UID of the process running the container is not known. As a result, a custom docker image had to be created that runs Erigon under root user.
- Snapshots for Erigon's nodes for many chains (including Ethereum) are downloaded using torrent. This process seems to be incredibly slow in an Akash deployment currently - possibly because there is no good way to open ports for torrent. In order to not have to wait many days for the node to sync with the blockchain, somewhat tricky workarounds had to be used, such as downloading the snapshots on a separate server first, mounting the persistent storage volume on Akash in a different folder, downloading the snapshots manually into the container, and then remounting the volume as Erigon data folder. Hopefully that can be avoided when spinning up additional nodes in the future.
