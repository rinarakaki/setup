# Install Node.js	

https://github.com/nodesource/distributions/blob/master/README.md#debmanual	

```sh
curl -fsSL https://deb.nodesource.com/gpgkey/nodesource.gpg.key | gpg --dearmor -o /usr/share/keyrings/nodesource-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/nodesource-archive-keyring.gpg] https://deb.nodesource.com/node_lts.x $VERSION_CODENAME main" > /etc/apt/sources.list.d/nodesource.list
apt update
apt install -y nodejs
npm install -g npm@latest
```
