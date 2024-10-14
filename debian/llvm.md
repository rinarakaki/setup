# Install LLVM	

https://apt.llvm.org/	

```sh
curl -s https://apt.llvm.org/llvm-snapshot.gpg.key | gpg --dearmor -o /usr/share/keyrings/llvm-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/llvm-archive-keyring.gpg] http://apt.llvm.org/$VERSION_CODENAME/ llvm-toolchain-$VERSION_CODENAME main" > /etc/apt/sources.list.d/llvm.list
apt update
apt install -y clang lldb lld
```
