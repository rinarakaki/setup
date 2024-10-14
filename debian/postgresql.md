# Install PostgreSQL

https://www.postgresql.org/download/linux/ubuntu/

```sh
curl -s https://www.postgresql.org/media/keys/ACCC4CF8.asc | gpg --dearmor -o /usr/share/keyrings/pgdg-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/pgdg-archive-keyring.gpg] http://apt.postgresql.org/pub/repos/apt/ $VERSION_CODENAME-pgdg main" > /etc/apt/sources.list.d/pgdg.list
apt update
apt install -y postgresql
```
