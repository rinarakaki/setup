# Install Helm

https://helm.sh/docs/intro/install/

```sh
ARCH=$(dpkg --print-architecture)
curl https://baltocdn.com/helm/signing.asc | gpg --dearmor -o /usr/share/keyrings/helm-archive-keyring.gpg
echo "deb [arch=$ARCH signed-by=/usr/share/keyrings/helm-archive-keyring.gpg] https://baltocdn.com/helm/stable/debian/ all main" > /etc/apt/sources.list.d/helm.list
apt update
apt install helm
```
