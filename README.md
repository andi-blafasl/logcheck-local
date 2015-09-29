# logcheck-local

I put my additions to logcheck rules under version control.

## how to use

1. clone this repo
2. link all files to /etc/logcheck/ignore.d.server
  
    cd /usr/local/etc/
    git clone https://github.com/andi-blafasl/logcheck-local.git
    chgrp logcheck logcheck-local
    cd /etc/logcheck/ignore.d.server
    for i in $(ls /usr/local/etc/logcheck-local/ | grep -v README); do ln -s /usr/local/etc/logcheck-local/$i $i; done
