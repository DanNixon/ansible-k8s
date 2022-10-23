# `dannixon.k8s.k3s_install`

Runs the K3s [install script](https://get.k3s.io/).
The most recent version (i.e. what is returned by the previous link) is used.

## Variables

- `k3s_install_options` (mapping): Environment variables to set when running script, see the link above for available options.

## Outputs

- `k3s_install_kubeconfig` (string): `kubeconfig` file used for access to the cluster.
