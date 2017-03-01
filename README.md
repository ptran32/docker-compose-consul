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

1) Download Image and create Image
```
sudo docker-compose build
```

2) Start all containers
```
sudo docker-compose up
```

3) Access to dashboard
```
http://localhost/8500/ui
```
