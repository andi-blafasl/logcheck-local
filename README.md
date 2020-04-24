# logcheck-local

I put my additions to logcheck rules under version control. Most of them are
designed for ubuntu (verion 14.04 and up) but also some rules for debian 7 are included.

## how to use

1. clone this repo
2. link all files to /etc/logcheck/ignore.d.server

```bash
cd /usr/local/etc/
git clone https://github.com/andi-blafasl/logcheck-local.git
chgrp logcheck logcheck-local
cd /etc/logcheck/ignore.d.server
for i in $(ls /usr/local/etc/logcheck-local/ | grep -v \.md); do ln -s /usr/local/etc/logcheck-local/$i local-$i; done
```
