# Kubefirst Charts

## Publishing a new chart

1. Update the version here https://github.com/kubefirst/charts/blob/main/charts/console/Chart.yaml
2. Run the following commands:
   - To create the packages (.tgz file): `helm package charts/*`
   - To update the index.yaml reference: `helm repo index --url https://kubefirst.github.io/charts/ .`
3. Open a PR against the `gh-pages` branch
4. Once the PR is merged, You can see the new package version here `https://kubefirst.github.io/charts/index.yaml`