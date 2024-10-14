# Install Terraform

- https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli

```sh
curl -s https://apt.releases.hashicorp.com/gpg |
    gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $VERSION_CODENAME main" > /etc/apt/sources.list.d/hashicorp.list
apt update
apt install terraform
```
