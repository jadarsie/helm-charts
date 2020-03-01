---
page_type: sample
languages:
- yaml
products:
- azure
description: "Sample Helm charts for Azure."
urlFragment: azure-helm-charts-sample
---

# Azure Samples - Helm Charts

## Configuration

Add the Azure Samples chart repository.

``` bash
helm repo add azure-samples https://raw.githubusercontent.com/jadarsie/helm-charts/master/docs/
```

## Chart source

All chart source material including chart readme files are found under the [chart-source directory](/chart-source/).

## Updating charts

``` bash
helm package chart-source/CHART_NAME -d docs/
helm repo index docs/ --url https://raw.githubusercontent.com/jadarsie/helm-charts/master/docs/
```
