# Machine

## Create

```shell
orbctl create --arch=arm64 --user=develop ubuntu:noble kubernetes
```

## Delete

```shell
orbctl delete kubernetes --force
```

# Ansible Ping

```shell
ansible all --inventory kubernetes.yaml --module-name ping
```

# Ansible Playbook nginx

```shell
ansible-playbook --inventory kubernetes.yaml playbooks/nginx.yaml
```

# Ansible Playbook kubernetes

```shell
ansible-playbook --inventory kubernetes.yaml playbooks/kubernetes.yaml
```

# Ansible Playbook kubeconfig

```shell
ansible-playbook --inventory kubernetes.yaml playbooks/kubeconfig.yaml
```

# Ansible Playbook kubeconfig_setup

```shell
ansible-playbook --inventory kubernetes.yaml playbooks/kubeconfig_setup.yaml
```

# Ansible Playbook untaint control plane

```shell
ansible-playbook --inventory kubernetes.yaml playbooks/k8s_untaint_control_plane.yaml
```

# Ansible Playbook helm

```shell
ansible-playbook --inventory kubernetes.yaml playbooks/helm.yaml
```

# Ansible Playbook cilium

```shell
ansible-playbook --inventory kubernetes.yaml playbooks/cilium.yaml
```

# Ansible Playbook ingress_nginx

```shell
ansible-playbook --inventory kubernetes.yaml playbooks/ingress_nginx.yaml
```

# Ansible Playbook local_path_provisioner

```shell
ansible-playbook --inventory kubernetes.yaml playbooks/local_path_provisioner.yaml
```

# Ansible Playbook cert_manager

```shell
ansible-playbook --inventory kubernetes.yaml playbooks/cert_manager.yaml
```
