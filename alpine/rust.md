- https://www.rust-lang.org/tools/install
- https://forge.rust-lang.org/infra/other-installation-methods.html

```sh
docker build \
    --output type=image,push=true \
    --platform linux/amd64,linux/arm64 \
    alpine/rust
```
