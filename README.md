# Portainer AWS ECR

### Create volume
```bash
    docker volume create portainer_data
    
    docker run -d -p 9000:9000 --name=portainer --restart=unless-stopped -v /var/run/docker.sock:/var/run/docker.sock -v portainer_data:/data portainer/portainer-ce
```

### Dockerize Nodejs App
```bash
    docker build . -t nodejs/node-web-app
    
    docker run -p 49160:8080 -d nodejs/node-web-app
```
