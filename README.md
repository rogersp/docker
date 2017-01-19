# docker

### Adding Windows routes

To communicate with docker containers directly from windows host, routes need to be added:

`route add -p 172.17.0.0 mask 255.255.0.0 10.0.75.2`

* `172.17.0.0` is the docker subnet
* `10.0.75.2` is the default IP of the docker VM, where the containers reside 
