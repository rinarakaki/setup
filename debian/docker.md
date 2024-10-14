# Install Docker

- https://docs.docker.com/engine/install/debian/
- https://docs.docker.com/engine/install/ubuntu/

```sh	
curl -fsSL https://download.docker.com/linux/$ID/gpg | gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
echo "deb [arch=amd64 signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/$ID $VERSION_CODENAME stable" > /etc/apt/sources.list.d/docker.list
apt update
apt install -y docker-ce-cli  # docker-ce containerd.io
```
