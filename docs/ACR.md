## Deploy a VMSS with at least 2 VMs

### kratentestvmss_bdde01f5 (10.1.0.5):

* Start server:

```bash
curl -sfL https://get.k3s.io | sh -

systemctl is-active k3s-server
```

* Get node token:

```bash 
 sudo cat /var/lib/rancher/k3s/server/node-token
```

### kratentestvmss_2f8896d3 (10.1.0.4):

* Start agent:
```bash
curl -sfL https://get.k3s.io | K3S_URL=https://$server:6443 K3S_TOKEN=$token sh -

systemctl is-active k3s-agent
``````               

## Deploy a k8s cluster on it using k3s

## Configure kraken to work with an ACR

## Deploy kraken helm app to the cluster

## Deploy a simple hello world app to the cluster 
