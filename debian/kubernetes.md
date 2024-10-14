# Install Kubernetes	

https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/	

```sh	
curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg |	
    gpg --dearmor -o /usr/share/keyrings/kubernetes-archive-keyring.gpg	
# TODO Waiting for `kubernetes-groovy` to be released	
echo "deb [signed-by=/usr/share/keyrings/kubernetes-archive-keyring.gpg] https://apt.kubernetes.io/ kubernetes-$VERSION_CODENAME main" > /etc/apt/sources.list.d/kubernetes.list	
apt update	
apt install -y kubectl	
```
