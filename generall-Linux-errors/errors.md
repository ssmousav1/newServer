

#####sudo: unable to resolve host `hostname`: Name or service not known 
- Edit `/etc/hosts` and append your new hostname to the 127.0.0.1 line (or create a new line if you prefer that).
 ```
127.0.0.1       localhost {hostname}
::1             localhost ip6-localhost ip6-loopback
ff02::1         ip6-allnodes
ff02::2         ip6-allrouters
```