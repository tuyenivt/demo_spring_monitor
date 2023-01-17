# demo_spring_monitor

## Start prometheus and grafana

`docker compose -f docker/docker-compose.yml up -d`

## Access to Prometheus

`http://localhost:9090/graph`

## Access to Grafana

`http://localhost:3000`

<p>Default login: <code>admin/admin</code></p>

## Add Prometheus data source to Grafana

<p>In Grafana, go to <code>Configuration > Data sources</code>, click on <code>Add data source</code></p>
<p>Select <code>Prometheus</code>, set <code>URL</code> to <code>http://prometheus:9090</code></p>
<p>Finish with <code>Save & test</code> button</p>

## Create Grafana Dashboards

<p>In Grafana, go to <code>Dashboards</code>, click on button <code>New</code> and select <code>Import</code>, under <code>Import via grafana.com</code></p>
<p>Load <code>https://grafana.com/grafana/dashboards/4701-jvm-micrometer</code></p>
<p>Load <code>https://grafana.com/grafana/dashboards/6083-spring-boot-hikaricp-jdbc</code></p>
<p>Load <code>https://grafana.com/grafana/dashboards/6756-spring-boot-statistics</code></p>
