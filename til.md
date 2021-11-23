### My TIL

1. [create an ssh tunnel on linux](#create-an-ssh-tunnel-on-linux)

### create an ssh tunnel on linux

```bash
$ ssh -N -L 3336:127.0.0.1:3306 [USER]@[SERVER_IP]
```

Used options are as follows:
- `-N` – tells SSH not to execute a remote command
- `-L` – creates port forwarding as follows: {local-port}:{remote-addr}:{remote-port}
