# Rumi DB

Rumi DB a configuration for the [PostgreSQL database packaged by Bitnami](https://github.com/bitnami/charts/tree/main/bitnami/postgresql/).

The configuration is aimed towards development on my workstation running [Minikube](https://minikube.sigs.k8s.io/docs/start/), mostly for hobby projects and experiments.

## Setup

> These instructions assume that you have a working [Minikube](https://minikube.sigs.k8s.io/docs/start/) install.

### Start PostgreSQL

```bash
helm upgrade --cleanup-on-fail --install postgresql bitnami/postgresql --namespace postgres --create-namespace --values postgresql.yaml
```

