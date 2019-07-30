# Kubernetes Ingress using Traefik

    2019 Ondrej Sika <ondrej@ondrejsika.com>
    https://github.com/ondrejsika/kubernetes-ingress-traefik

Simplest way, how to setup Ingress with Let's Encrypt certificates.


## Features

- Automatic HTTP to HTTPS redirect
- SSL using Let's Encrypt web challenge


## Install to Kubernetes

Apply locally

```
kubect apply -f ingress-traefik.yml
```

or from Github's master

```
kubect apply -f https://raw.githubusercontent.com/ondrejsika/kubernetes-ingress-traefik/master/ingress-traefik.yml
```