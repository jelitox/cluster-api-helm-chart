# Cluster API Helm Chart
A Helm chart to install Cluster API manifests 

* Installs the [cluster API Manifests](cluster-api.sigs.k8s.io).

*Note: Currently the chart install a target cluster in AWS. However it is intended to incude the support for other Cluster API providers.*


## Installing the Chart using ArgoCD

More details: https://github.com/kgamanji/cluster-api-argocd

To install the chart using ArgoCD use the following command:
```
kubectl apply -f argocd/application-capi.yaml
```

## Installing the Chart

To install the chart with the release name `my-release`:

***TO BE IMEPMELENTED*** 
```bash
## helm install kgamanji/cluster-api-aws
```


## Configuration

| Parameter                                    | Description                                                                           | Default                                    |
|:---------------------------------------------|:--------------------------------------------------------------------------------------|:-------------------------------------------|
| `kube.version`                           | Kubernetes version to be installed on the target clusters                                 | `v1.18.8`        |
| `controlPlane.replicas`                                  | Amount of master nodes in the target cluster                                                     | `3`                                   |
| `workers.replica`                           | Amount of worker nodes in the target cluster                                                                    | `3`                             |
