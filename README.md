# 10-monitoring-03-grafana

## Задание 1
<img width="880" height="960" alt="image" src="https://github.com/erant-netology-courses/10-monitoring-03-grafana/blob/main/1.JPG?raw=true" />

## Задание 2
```
100 - (avg(rate(node_cpu_seconds_total{mode="idle"}[1m])) * 100)
node_load1; node_load5; node_load15
node_memory_MemFree_bytes / 1024 / 1024 / 1024
node_filesystem_free_bytes{mountpoint="/"}
```

<img width="1580" height="960" alt="image" src="https://github.com/erant-netology-courses/10-monitoring-03-grafana/blob/main/2_dashboard.JPG?raw=true" />

## Задание 3

Я настроил интеграцию с ТГ, но она не отрабатывала. Спустя час дебага вспомнил, что яндекс на российских серверах, а в РФ заблокирован ТГ. Делал через alertmanager и внутри графаны (сперва вообще там, но там не отработала отправка тестового сообщения).

Исходники настроек alertmanager в репозитории.

## Задание 4

[Файл с логами](https://github.com/erant-netology-courses/10-monitoring-03-grafana/blob/main/dashboard-1781433617181.json?raw=true)