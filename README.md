# One Beyond - Helm Charts repository

- [One Beyond - Helm Charts repository](#one-beyond---helm-charts-repository)
  - [Usage](#usage)
  - [Charts](#charts)
    - [one-beyond-cronjob](#one-beyond-cronjob)
    - [one-beyond-cronjob-http](#one-beyond-cronjob-http)

## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

```
  helm repo add onebeyond https://onebeyond.github.io/helm-charts
```

If you had already added this repo earlier, run `helm repo update` to retrieve
the latest versions of the packages.  You can then run `helm search repo
onebeyond` to see the charts.

## Charts

### one-beyond-cronjob

To install the one-beyond-cronjob chart:

```
    helm install my-test-cronjob onebeyond/one-beyond-cronjob
```

To uninstall the chart:

```
    helm delete my-test-cronjob
```
### one-beyond-cronjob-http

This cronjob will do a request using curl to trigger actions, webhooks, etc

Please check [values.yaml](https://github.com/onebeyond/helm-charts/blob/main/charts/one-beyond-cronjob-http/values.yaml) for possible configuration values.

To install the one-beyond-cronjob-http chart:

```
    helm install my-test-cronjob-http onebeyond/one-beyond-cronjob-http
```

To uninstall the chart:

```
    helm delete my-test-cronjob-http
```
