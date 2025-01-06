# Install Cloud SQL Auth Proxy

- https://cloud.google.com/sql/docs/mysql/sql-proxy#linux-64-bit
- https://github.com/GoogleCloudPlatform/cloud-sql-proxy

```sh
VERSION=v2.14.1
ARCH=$(dpkg --print-architecture)
curl -o /usr/local/bin/cloud-sql-proxy https://storage.googleapis.com/cloud-sql-connectors/cloud-sql-proxy/$VERSION/cloud-sql-proxy.linux.$ARCH
chmod +x /usr/local/bin/cloud-sql-proxy
```
