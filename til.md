### My TIL

1. [create an ssh tunnel on linux](#create-an-ssh-tunnel-on-linux)
2. [create db in PostgreSQL](#create-db-in-postgresql)
3. [create user in PostgreSQL](#create-user-in-postgresql)
4. [grant privilages in PostgreSQL](#grant-privilages-in-postgresql)

### create an ssh tunnel on linux

```bash
$ ssh -N -L 3336:127.0.0.1:3306 [USER]@[SERVER_IP]
```

Used options are as follows:
- `-N` – tells SSH not to execute a remote command
- `-L` – creates port forwarding as follows: {local-port}:{remote-addr}:{remote-port}

### create db in PostgreSQL
```sql
CREATE DATABASE <dbname>;
```

### create user in PostgreSQL
```sql
CREATE USER <dbuser> WITH ENCRYPTED PASSWORD '<dbpass>';
```

### grant privilages in PostgreSQL
```sql
GRANT ALL PRIVILEGES ON DATABASE <dbname> TO <dbuser>;
```
