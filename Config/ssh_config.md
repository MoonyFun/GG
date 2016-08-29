##ssh config

```
*远程ssh设置*

Host alias
    HostName 1.1.1.1
    User    root
    Port    8888
    
*多个ssh key设置*

Host www.xxxx.com
    HostName 1.1.1.1
    User   name
    IdentityFile ~/.ssh/key-file
    
```