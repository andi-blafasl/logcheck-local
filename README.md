# logcheck-local

I put my additions to logcheck rules under version control.

## how to use

1. clone this repo
2. link all files to /etc/logcheck/ignore.d.server
  
    cd /root/
    git clone https://github.com/andi-blafasl/logcheck-local.git
    for i in $(ls /root/logcheck.local/*); do ln -s /root/logcheck.local/$i $i; done

