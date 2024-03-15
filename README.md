# Kubefirst Charts


## Bump Macro Chart

1. adjust [console version](https://github.com/kubefirst/charts/blob/main/charts/kubefirst/Chart.yaml#L5) (if needed)
2. adjust [kubefirst-api version](https://github.com/kubefirst/charts/blob/main/charts/kubefirst/Chart.yaml#L8) (if needed)
3. adjust [macro chart version](https://github.com/kubefirst/charts/blob/main/charts/kubefirst/Chart.yaml#L16)
4. generate helm package

```bash 
helm dependency update ./charts/kubefirst
```
5. Open a PR against the `main` branch
6. Once you merge the PR the GitHub action will update the chart in the Kubefirst Chart Museum

## Adding Kubefirst chart to the Helm repo

Run the following commands

```bash 
helm repo add kubefirst https://charts.kubefirst.com
helm repo update 
```

## Installing Kubefirst chart

replace <version> with the desired version  
```bash
helm install kubefirst --create-namespace --version <version> kubefirst/kubefirst
```
