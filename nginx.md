Like Github, Docker has its community on DockerHub, it include both official anduser-submitted docker images.

### Downloading Nginx from DockerHub
```
docker pull nginx
```

To make it accessible to public as a web server, configure the container as follows:
```
docker run --name nginx-docker -p 80:80 nginx
```	

>>run public ip on your browser, welcom NGINX page will appear
>>in your terminal press CTRL+C to exit from docker run command
>> NOw rmove docker by following command:
```
docker rm nginx-docker
```

### Detachment Mode
Run docker in Detachment Mode by:
```
docker run --name nginx-docker -p 80:80 -d nginx
```

### CReate a custom web page
```
mkdir -p ~/nginx-docker/html
cd ~/nginx-docker/html
```

Create a html file:
```
nano index.html
```
Insert the following Code
```
<html>
  <head>
    <title>Docker nginx Tutorial</title>
  </head>

  <body>
    <div class="container">
      <h1>Hello DigitalOcean</h1>
      <p>This Nginx page is brought to you by Docker and DigitalOcean</p>
    </div>
  </body>
</html>
```

run docker:
```
docker run --name docker-nginx -p 80:80 -d -v ~/docker-nginx/html:/usr/share/nginx/html nginx
```

