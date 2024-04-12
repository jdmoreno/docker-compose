Configuration

Before starting the cluster, let’s create the network we are going to use to communicate our cluster to our monitoring stack. 
This change allows us create multiple docker-compose files to isolate our services based on their responsibilities. It will help avoid having a big docker-compose with multiple services doing different things.

```sh
docker network create kafka
```

