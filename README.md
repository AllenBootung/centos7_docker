Using systemctl in docker

1.download and build this Dockerfile
#docker build --rm -t local/c7-systemd .

2.run image in background
#docker run --privileged -tid -e "container=docker" -v /sys/fs/cgroup:/sys/fs/cgroup local/c7-systemd /usr/sbin/init

3.find container id
#docker ps -a

4.exec container s398sd0323rsefs3rsf3
#docker exec -ti s39 bash