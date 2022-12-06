# Kubescape Operator

This repository contains a Juju Charm for deploying Kubescape on Kubernetes.

## Usage

Kubescape may be deployed to a Kubernetes cluster via Juju as following:

```
charmcraft pack
```

```
juju add-model kubescape
```

```
juju deploy --trust ./kubescape-charmed_ubuntu-22.04-amd64.charm --config clusterName=`kubectl config current-context` --config account=<YOUR_KUBESCAPE_ACCOUNT_ID>
```
