# Heva Helm Charts

## Getting started

```
helm repo add helm-charts https://fozdoiguassu.github.io/helm-charts/
helm search repo helm-charts
```

## Charts

* [Hive-metastore](./charts/hive-metastore/README.md): Deploy [Hive](https://hive.apache.org/) metastore


## Contributing

### Requirements
* https://github.com/helm/chart-testing
* https://github.com/bitnami/readme-generator-for-helm

### CI

Run linter in chart directory:
```
ct lint --chart-dirs . --charts .
```

Update chart parameters in readme
```
readme-generator -v values.yaml -r README.md
```

Update README table of contents
```
npx markdown-toc -i README.md --bullets '-'
```
