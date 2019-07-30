# Kubernetes Ingress using Traefik

    2019 Ondrej Sika <ondrej@ondrejsika.com>
    https://github.com/ondrejsika/kubernetes-ingress-traefik

Simplest way, how to setup Ingress with Let's Encrypt certificates.


## Features

- Automatic HTTP to HTTPS redirect
- SSL using Let's Encrypt web challenge

## Requirements

### Default StorageClass

If you don't have any Storage provisioner, you can install [local-path-provisioner](https://github.com/rancher/local-path-provisioner)

```
kubectl apply -f https://raw.githubusercontent.com/rancher/local-path-provisioner/master/deploy/local-path-storage.yaml
kubectl patch storageclass local-path -p '{"metadata": {"annotations":{"storageclass.kubernetes.io/is-default-class":"true"}}}'
```

## Install Traefik Ingress to Kubernetes

Apply locally

```
kubect apply -f ingress-traefik.yml
```

or from Github's master

```
kubect apply -f https://raw.githubusercontent.com/ondrejsika/kubernetes-ingress-traefik/master/ingress-traefik.yml
```