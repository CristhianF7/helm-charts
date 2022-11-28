# Kubefirst Charts

## Publishing a new chart

1. Update the version here [Chart version](https://github.com/kubefirst/charts/blob/main/charts/console/Chart.yaml)
2. Run the following commands:
   - To create the packages (.tgz file): `helm package charts/*`
   - To update the index.yaml reference: `helm repo index --url https://cristhianf7.github.io/helm-charts/ .`
3. Open a PR against the `gh-pages` branch
4. Once the PR is merged, You can see the new package version here [Kubefirst Chart Repository](https://kubefirst.github.io/charts/index.yaml)


### Adding helm chart to you repo

helm repo add api https://kubefirst.github.io/charts/
helm repo add console https://kubefirst.github.io/charts/