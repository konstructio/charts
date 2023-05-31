# Kubefirst Charts

## Publishing a new chart

1. Update the version here [Chart version](https://github.com/kubefirst/charts/blob/main/charts/console/Chart.yaml)
2. Open a PR against the `main` branch
3. Once you merge the PR the GitHub action will update the chart in the `gh-pages` branch and then publish using GitHub pages.

You can see the new package version here [Kubefirst Chart Repository](https://kubefirst.github.io/charts/index.yaml)

### Adding helm chart to you repo

helm repo add kubefirst https://charts.kubefirst.com
