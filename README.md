Dockerized RTBkit zookeeper
======

```
sudo docker build -t onokonem/rtbkit-zookeeper https://github.com/onokonem/rtbkit-zookeeper-docker.git

sudo docker run \
  -d --net=host \
  -v /storage/docker/zookeeper/data:/zookeeper-data \
  -p 2181:2181 \
  onokonem/rtbkit-zookeeper
```