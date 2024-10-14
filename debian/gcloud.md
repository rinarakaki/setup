# Install Google Cloud SDK	

https://cloud.google.com/sdk/docs/install	

```sh	
curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | gpg --dearmor -o /usr/share/keyrings/cloud-google-sdk-archive-keyring.gpg	
echo "deb [signed-by=/usr/share/keyrings/cloud-google-sdk-archive-keyring.gpg] http://packages.cloud.google.com/apt cloud-sdk main" > /etc/apt/sources.list.d/google-cloud-sdk.list	
apt update	
apt install -y google-cloud-sdk	
```
