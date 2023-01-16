# demo_spring_monitor

## Start prometheus and grafana

`docker compose -f docker/docker-compose.yml up -d`

## Access to Prometheus

`http://localhost:9090/graph`

## Access to Grafana

`http://localhost:3000`

<p>Default login: admin/admin</p>

## Add Prometheus data source to Grafana

<p>In Grafana, go to `Configuration > Data sources`, click on `Add data source`</p>
<p>Select `Prometheus`, set `URL` to `http://prometheus:9090`</p>
<p>Finish with `Save & test` button</p>

## Create Grafana Dashboards

<p>In `Grafana`, go to `Dashboards`, click on button `New` and select `Import`, under `Import via grafana.com`</p>
<p>Load `https://grafana.com/grafana/dashboards/4701-jvm-micrometer`</p>
<p>Load `https://grafana.com/grafana/dashboards/6083-spring-boot-hikaricp-jdbc`</p>
<p>Load `https://grafana.com/grafana/dashboards/6756-spring-boot-statistics`</p>
