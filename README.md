# tomandfriends
docker run -d --name proxy --net=host --hostname=proxy -v /cache:/cache -v ./nginx_conf:/etc/nginx/conf.d -v ./www :/var/www/:ro  nginx

docker run -d --name proxy_2 --net=host --hostname=proxy -v /cache:/cache -v /root/deploy/nginx_conf:/etc/nginx/conf.d:ro -v /root/deploy/www:/var/www/:ro  nginx2