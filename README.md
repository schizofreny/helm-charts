# helm-charts

## Usage

```sh
# add our repository
helm repo add schizofreny https://schizofreny.github.io/helm-charts

# update stuff from repo
helm repo update

# use some chart like this schizofreny/$CHART_NAME
helm install --generate-name schizofreny/httpbin
```

## Contributing

To add chart, simply add valid chart to `charts/$CHART_NAME` folder. On push to master, all new charts and chart versions will be released to github pages.

To release new chart version, simply bump up `version` in `Chart.yaml`.

Also it is ideal to use pull requests, because there are included github actions that lint changed helm chart files.
