Grafana + Influx Timeshift Proxy
---
Install:
clone https://github.com/IovetsNikolay/grafana_timeshift
docker-compose pull
docker-compose build 
docker-compose down
docker-compose up -d
---
Check:
docker ps --->
grafana/grafana     "bash -x /run1.sh"       0.0.0.0:8857->3000/tcp   grafana
node:alpine         "docker-entrypoint.s…"   8989/tcp                 influxdb-timeshift-proxy
---
Sources:
https://github.com/serputko/performance-testing-framework
https://github.com/maxsivanov/influxdb-timeshift-proxy
