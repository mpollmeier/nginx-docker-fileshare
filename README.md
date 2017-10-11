# Docker commands
docker build -t mpollmeier/nginx-fileshare .
docker push mpollmeier/nginx-fileshare
docker run -p 8080:80 -v /path/on/host:/usr/share/nginx/html:ro -d mpollmeier/nginx-fileshare
