git clone https://github.com/djratza/openhab2-docker.git

tar -xvzf openahn2.tar.gz

docker build -t "openhab2" .

docker run --rm --device /dev/gpiomem -p 1234:8080 -dt openhab2

docker exec -it containerID tail -f /var/log/openhab2/*

when openhan2 runs choose Expert mode

Install exec binding, onewiregpio, opencloud
