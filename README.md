# demo_spring_monitor

## Start `prometheus` and `grafana`

`docker compose -f docker/docker-compose.yml up -d`

## Access `Prometheus`

`http://localhost:9090/graph`

## Access `Grafana`

`http://localhost:3000`

Default login: admin/admin

## Add `Prometheus` data source to `Grafana`

In `Grafana`, go to `Configuration` > `Data sources`, click on `Add data source`
Select `Prometheus`, set `URL` to `http://prometheus:9090`
Finish with `Save & test` button

## Create `JVM (Micrometer) Dashboard` Grafana

In `Grafana`, go to `Dashboards`, click on button `New` and select `Import`
Load `https://grafana.com/grafana/dashboards/4701-jvm-micrometer` under `Import via grafana.com`

## Create `Database Connection Dashboard` dashboard

In `Grafana`, go to `Dashboards`, click on button `New` and select `Import`
Load `https://grafana.com/grafana/dashboards/6083-spring-boot-hikaricp-jdbc` under `Import via grafana.com`
