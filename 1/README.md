## Grafana + Prometheus

### variant 1: manual configuration

Run this with:<br>
`docker compose up`<br>

And then open in browser:<br>
* Grafana - 127.0.0.1:3001 (login with credentials "admin" : "grafana")
* Prometheus - 127.0.0.1:9091

grafana and prometheus are available but not connected<br>


### variant 2: add persistent volume for Prometheus data

`docker compose -f compose-full.yml up -d`<br>
AND for this case do the following after use (clean with volumes)<br>
`docker compose -f compose-full.yml down -v`<br>

As in the previous example, both services can be opened in browser<br>


### variant 3: add Node Exporter for data collection

replace target IP adress from '192.168.1.12' to your host OS IP in this_repo/1/1/prometheus/prometheus.yml<br>

```
cd 1
docker compose up -d
```

As in the previous examples, both services can be opened in browser<br>
and it will use one more container with Node Exporter<br>
you can see it in browser: http://localhost:9100/metrics<br>

