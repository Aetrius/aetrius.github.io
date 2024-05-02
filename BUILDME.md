## Package Chart
helm package msockperf

mkdir charts

mv msockperf-chart-0.1.5.tgz charts/msockperf-chart-.0.1.92.tgz

cp infra/k8s/base/app/msockperf-chart/index.yaml index.yaml

## Gather sha256sum
sha256sum msockperf/charts/msockperf-chart-0.1.92.tgz | awk '{ print $1 }'

## GZIP YAML
gzip -f index.yaml


## UNZIP Yaml
gunzip index.yaml.gz