

# INSTALL CHART
    ` 
        helm install msockperf msockperf -f msockperf/env/values.local.yaml --namespace msockperf --create-namespace

        helm upgrade msockperf msockperf -f msockperf/env/values.local.yaml --namespace msockperf  

    `

