# sikalabs-kubernetes-ingress (Ingress using Traefik)

    2019 Ondrej Sika <ondrej@ondrejsika.com>
    https://github.com/sikalabs/sikalabs-kubernetes-ingress

Simple way, how to setup Ingress with Let's Encrypt certificates & Prometheus Metrics.

## Install Traefik Ingress to Kubernetes

Apply locally

```
kubectl apply -f ingress-traefik.yml
```

or from Github's master

```
kubectl apply -f https://raw.githubusercontent.com/sikalabs/sikalabs-kubernetes-ingress/master/ingress-traefik.yml
```
