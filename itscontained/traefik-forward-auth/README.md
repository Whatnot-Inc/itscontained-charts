# traefik-forward-auth Helm Chart

This is a helm chart for [traefik-forward-auth](https://github.com/thomseddon/traefik-forward-auth) 

The default values and container images used in this chart will allow for running in a multi-arch cluster (amd64, arm, arm64)

## TL;DR

```console
helm repo add billimek https://billimek.com/billimek-charts/
helm install billimek/traefik-forward-auth
```

## Installing the Chart

To install the chart with the release name `traefik-forward-auth`:

```console
helm install traefik-forward-auth billimek/traefik-forward-auth
```

## Uninstalling the Chart

To uninstall/delete the `traefik-forward-auth` deployment:

```console
helm uninstall traefik-forward-auth
```

The command removes all the Kubernetes components associated with the chart and deletes the release.

## Configuration

Read through the [values.yaml](https://github.com/billimek/billimek-charts/blob/master/charts/traefik-forward-auth/values.yaml) file. It has several commented out suggested values.

Specify each parameter using the `--set key=value[,key=value]` argument to `helm install`. For example,

```console
helm install traefik-forward-auth \
  --set timeZone="America/New York" \
    billimek/traefik-forward-auth
```

Alternatively, a YAML file that specifies the values for the above parameters can be provided while installing the chart. For example,

```console
helm install traefik-forward-auth billimek/traefik-forward-auth  --values values.yaml 
```