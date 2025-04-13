# Install Kubernetes

https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/

```sh
curl -fsSL https://pkgs.k8s.io/core:/stable:/v1.32/deb/Release.key |
    gpg --dearmor -o /usr/share/keyrings/kubernetes-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/kubernetes-archive-keyring.gpg] https://pkgs.k8s.io/core:/stable:/v1.32/deb/ /" > /etc/apt/sources.list.d/kubernetes.list
apt update
apt install -y kubectl
```
