References
https://docs.docker.com/compose/environment-variables/
https://stackoverflow.com/questions/65935051/how-can-i-pass-host-ip-address-to-docker-compose-file
https://stackoverflow.com/questions/29377853/how-can-i-use-environment-variables-in-docker-compose/33186458#33186458
https://modulitos.com/blog/lets-deploy-part-1/


Configuration

Before starting the cluster, let’s create the network we are going to use to communicate our cluster to our monitoring stack. 
This change allows us create multiple docker-compose files to isolate our services based on their responsibilities. It will help avoid having a big docker-compose with multiple services doing different things.

```sh
docker network create kafka
```

