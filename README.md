# [Docker Getting Started Tutorial](https://docs.docker.com/get-started/)

## requiements
[Docker Dosktop](https://www.docker.com/)
[Accout Docker Hub](https://hub.docker.com/)

## Getting Started

1. Before you can run the application, you need to get the application source code onto your machine:

```bash
git clone https://github.com/BossHunTerCoding/docker-get-start.git
```

2. In the `app` directory, the same location as the `package.json` file,  `Dockerfile`. In the Windows Command Prompt, run the following commands listed below:
```bash
cd docker-get-start/app/
```

3. Build the container image. (In terminal much In the `app` directory), with the fields enclosed by brackets "{}" replaced with your fields. (Don't include the brackets!):
```bash
docker build -t {the_name_image} .
```

4. Start your container using the docker run command and specify the name of the image you just created. (In terminal much In the `app` directory), with the fields enclosed by brackets "{}" replaced with your fields. (Don't include the brackets!):
```bash
docker run --name {the_name_container} -dp {portout}:3000 {the_name_image}
```

5. Update the source code, can update in `app>src` (In terminal much In the `app` directory)
check list docker:
```bash
docker ps -l
```
container much stop running, with the fields enclosed by brackets "{}" replaced with your fields. (Don't include the brackets!):
```bash
docker stop {CONTAINER ID}
```
remove container, with the fields enclosed by brackets "{}" replaced with your fields. (Don't include the brackets!):
```bash
docker rm {CONTAINER ID}
```
update image, with the fields enclosed by brackets "{}" replaced with your fields. (Don't include the brackets!):
```bash
docker build -t {the_same_name_image_your_build} .
```
start container again, with the fields enclosed by brackets "{}" replaced with your fields. (Don't include the brackets!):
```bash
docker run --name {the_name_container} -dp {portout}:3000 {the_name_image}
```