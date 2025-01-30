# Asterisk

- https://docs.asterisk.org/Getting-Started/Installing-Asterisk/Installing-Asterisk-From-Source/What-to-Download/
- https://algostore.com/blog/post/asterisk-installation-on-ubuntu-1804

```sh
ASTERISK_VERSION=22
apt install wget build-essential libedit-dev uuid-dev libjansson-dev libxml2-dev libsqlite3-dev
wget https://downloads.asterisk.org/pub/telephony/asterisk/asterisk-$ASTERISK_VERSION-current.tar.gz
tar xvf asterisk-$ASTERISK_VERSION-current.tar.gz
cd asterisk-$ASTERISK_VERSION.*
./configure
make
```
