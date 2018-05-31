# alpine-nginx-docker


### コマンド  

docker build -f alpine-nginx.dockerfile -t nginx .  
echo 'hello, world' > index.html  
docker run -d -p 8080:80 -v $(pwd):/usr/share/nginx/html nginx  
curl http://$(docker-machine ip default):8080　または　curl http://localhost:8080  
