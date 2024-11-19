# Linux Command
## Tunnel over SSH

```commandline
ssh -L [bind_address:]port:host:host_port user@hostname [-N]
```

| option       | description                   |
|--------------|-------------------------------|
| bind_address | local address to bind to      |
| port         | local port to bind to         |
| host         | remote host to connect to     |
| host_port    | remote port to connect to     |
| -N           | do not execute remote command |

Example : Forward remote port 8080 to local port 9000
```commandline
ssh -L 9000:localhost:8080 user@remote -N
```


