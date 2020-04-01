#### first copy ssh public key
```bash
cat ~/.ssh/id_rsa.pub > authorized_keys
```

#### then run compose
```bash
docker-compose up -d --build
```

#### finally, connect to container with ssh
```bash
ssh -p 2222 root@localhost
ssh -p 2223 root@localhost
```