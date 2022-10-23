# `dannixon.k8s.grafana_agent`

Deploys [Grafana Agent](https://grafana.com/docs/agent/latest/) on a Kuberenets cluster for metrics and log collection.

See the [metrics](https://grafana.com/docs/grafana-cloud/kubernetes-monitoring/agent-k8s/k8s_agent_metrics/) and [log](https://grafana.com/docs/grafana-cloud/kubernetes-monitoring/agent-k8s/k8s_agent_logs/) collection quickstarts for configuration information.

## Variables

- `grafana_agent_version` (string): Version of Grafana Agent to deploy.
- `grafana_agent_metrics_enable` (bool): If metrics collection should be enabled.
- `grafana_agent_metrics_namespace` (string): Namespace in which to deploy metrics collection.
- `grafana_agent_metrics_config` (string): YAML configuration for metrics collection.
- `grafana_agent_logs_enable` (bool): If log collection should be enabled.
- `grafana_agent_logs_namespace`(string): Namespace in which to deploy log collection.
- `grafana_agent_logs_config` (string): YAML configuration for logs collection.
