- operator for k8s
- neat trick to allow dns queries to swithc between resolvers:
  ---
  in /etc/resolve/conf:
    options rotate
    options timeout:1
    search xyz.abc.local
    nameserver 192.168.56.3
    nameserver 10.0.2.4
  ---