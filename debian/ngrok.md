# ngrok

- https://download.ngrok.com/downloads/linux

```sh
curl -sSL https://ngrok-agent.s3.amazonaws.com/ngrok.asc > /etc/apt/trusted.gpg.d/ngrok.asc
echo "deb https://ngrok-agent.s3.amazonaws.com buster main" > /etc/apt/sources.list.d/ngrok.list
apt update
apt install ngrok
```
