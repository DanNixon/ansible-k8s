# `dannixon.k8s.grafana_agent`

Deploys [Grafana Agent](https://grafana.com/docs/agent/latest/) on a Kuberenets cluster for metrics and log collection.

See the [metrics](https://grafana.com/docs/grafana-cloud/kubernetes-monitoring/agent-k8s/k8s_agent_metrics/) and [log](https://grafana.com/docs/grafana-cloud/kubernetes-monitoring/agent-k8s/k8s_agent_logs/) collection quickstarts for configuration instructions.
Note that the `ConfigMap` for metrics and log configs must use the defaults of `grafana-agent` and `grafana-agent-logs` respectively.

## Variables

- `grafana_agent_version` (string): version of Grafana Agent to deploy
- `grafana_agent_metrics_enable` (bool): if metrics collection should be enabled
- `grafana_agent_metrics_namespace` (string): namespace in which to deploy metrics collection
- `grafana_agent_logs_enable` (bool): if log collection should be enabled
- `grafana_agent_logs_namespace`(string): namespace in which to deploy log collection
