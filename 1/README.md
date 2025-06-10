## Grafana + Prometheus

Run this with:<br>
`docker compose up`<br>

OR<br>
`docker compose -f compose-full.yml up -d`<br>
AND for this case do the following after use (clean with volumes)<br>
`docker compose -f compose-full.yml down -v`<br>


And then open in browser:<br>
* Grafana - 127.0.0.1:3001 (login with credentials "admin" : "grafana")
* Prometheus - 127.0.0.1:9091
