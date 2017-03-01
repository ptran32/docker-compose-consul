# puppet-box

#OS and Virtualization:

Ubuntu 16.04 & docker-compose version 1.11.2

#What this docker-compose do?

This docker-compose creates three containers:

- consul-server (with web UI integrated)
- consul-client-1
- consul-client-2

#Requirements:

Vagrant installed

#How to use docker-compose?

Download Image and create Image
```
sudo docker-compose build
```

Start all containers
```
sudo docker-compose up -d
```
Check containers status
```
sudo docker-compose ps
```
Access to dashboard
```
http://localhost/8500/ui
```
Stop and remove all containers
```
sudo docker-compose stop && sudo docker-compose rm
```

