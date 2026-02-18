### Implement Nodejs web service to learn docker .

#### Steps
1. Install docker .

2. Clone the repository :
```shell
git clone https://github.com/Ho3einTahan/First-Nodejs-Docker
cd First-Nodejs-Docker
```

3. Build Docker File :
```shell
docker build -t my-node-app .
```

4. Run the docker container :
```shell
docker run -p 3000:3000 my-node-app
```

5. See all runing containers :
```shell
docker ps
```

#### ⚠️ Troubleshooting
##### If you see this error:
```plainText
Error: listen EADDRINUSE: address already in use :::3000
```
##### It means port 3000 is already in use on your system. You have two options:
1. Change the port in run command
```shell
docker run -p 3001:3000 my-node-app
```
2. Modify the EXPOSE line in Dockerfile:
```plain
EXPOSE 3001
```

### Author
#### Developed By Ho3ein Tahan