# Ansible Role: arillso.agents.grafana

## Description

The role installs the Grafana Agent and configures it.

## Role Variables

### grafana_server

All the configuration options for the `grafana_server` section and `server_config` respectively
can be found on the documentation page of Grafana Labs:

<https://grafana.com/docs/agent/latest/configuration/server-config/>

#### defaults grafana_server

```yml
grafana_server:
  log_level: warn
```

### grafana_metrics

All the configuration options for the `grafana_metrics` section and `metrics_config` respectively
can be found on the documentation page of Grafana Labs:

<https://grafana.com/docs/agent/latest/configuration/metrics-config/>

#### defaults grafana_metrics

```yml
grafana_metrics:
  global:
    scrape_interval: 1m
  configs:
    - name: integrations
```

### grafana_integrations

All the configuration options for the `grafana_integrations` section and `integrations_config` respectively
can be found on the documentation page of Grafana Labs:

<https://grafana.com/docs/agent/latest/configuration/integrations/>

#### defaults grafana_integrations

```yml
grafana_integrations:
  agent:
    enabled: true
```

#### grafana_logs

All the configuration options for the `grafana_logs` section and `logs_config` respectively
can be found on the documentation page of Grafana Labs:

<https://grafana.com/docs/agent/latest/configuration/logs-config/>

#### defaults grafana_logs

```yml
grafana_logs:
  positions_directory: "C:\\ProgramData\\grafana-agent-logs"
```
