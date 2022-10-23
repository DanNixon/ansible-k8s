# `dannixon.k8s.cilium`

Deploys [Cilium](https://cilium.io/) with a somewhat opinionated configuration.

Specifically:

- Configures host firewall (see [`node.yml`](./tasks/node.yml))
- Deploys Cilium [via Helm](https://docs.cilium.io/en/stable/gettingstarted/k8s-install-helm/) (see [`deploy.yml`](./tasks/deploy.yml))

Uses the following high level configuration:

- WireGuard inter-node communication
- Hubble (relay and UI) enabled
- Cilium Prometheus metrics enabled
