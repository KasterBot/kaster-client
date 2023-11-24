# kaster-client
KasterBot client

## Introduction

KasterBot is your cloud and DevOps assistant that you can chat with to help you manage your infrastructure, including linux servers, and kubernetes clusters. KasterBot is powered by GPT-4.

## How to use?
Choose a plan in RapidAPI and install the kaster-client in your k8s cluster and/or your linux server.

### Install kaster-client on k8s cluster

```helm repo add kasterbot https://kasterbot.github.io/kaster-client```

```helm repo update kasterbot```

Create a yaml file `custom.yaml` and type this code:
```yaml
env:
  value: "<X-RapidAPI-Key>"

```

```
helm install kaster-client kasterbot/kaster -f custom.yaml 
```
