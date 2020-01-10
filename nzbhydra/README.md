nzbhydra
========
A Helm chart for Kubernetes

Current chart version is `0.1.5`





## Chart Values

| Key | Type | Default | Description |
|-----|------|---------|-------------|
| fullnameOverride | string | `""` |  |
| image.pullPolicy | string | `"Always"` |  |
| image.repository | string | `"registry.holthome.net/k8s-services/docker-nzbhydra"` |  |
| image.tag | string | `"latest"` |  |
| ingress.annotations | object | `{}` |  |
| ingress.enabled | bool | `false` |  |
| ingress.hosts[0] | string | `"chart-example.local"` |  |
| ingress.path | string | `"/"` |  |
| ingress.tls | list | `[]` |  |
| nameOverride | string | `""` |  |
| nzbhydra.configDir | string | `"/config"` |  |
| nzbhydra.downloadDir | string | `"/downloads"` |  |
| nzbhydra.env.PGID | int | `50000` |  |
| nzbhydra.env.PUID | int | `50000` |  |
| nzbhydra.env.TZ | string | `"America/New_York"` |  |
| persistence.config.accessMode | string | `"ReadWriteOnce"` |  |
| persistence.config.enabled | bool | `true` |  |
| persistence.downloads.existingClaim | string | `"tank-docker-pvc"` |  |
| persistence.downloads.subPath | string | `"root"` |  |
| podAnnotations | object | `{}` |  |
| replicaCount | int | `1` |  |
| resources | object | `{}` |  |
| service.port | int | `5076` |  |
| service.type | string | `"ClusterIP"` |  |
| storageClassName | string | `"slow-disks"` |  |
| strategyType | string | `"Recreate"` |  |
