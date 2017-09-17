# Flask App in Docker
Build a docker image from a flask app and run in a docker container

## Basic Commands
Create image using directory's Dockerfile   `docker build -t tagname`

Run "tagname" on port 4000 to 80   `docker run -p 4000:80 tagname`

List all running containers   `docker container ls`

List all containers, even non-running ones   `docker container ls -a`

Gracefully stop specified container   `docker container stop <hash>`

Remove specified container   `docker container rm <hash>`

Remove all containers   `docker container rm $(docker container ls -aq)`

List all images on machine   `docker image ls -a`

Remove specified image from machine   `docker image rm <image-id>`

Remove all images from machine   `docker image rm $(docker image ls -aq)`

Tag image for upload to registry   `docker tag <image> username/repository:tag`

Upload tagged image to registry   `docker push username/repository:tag`

Run image from registry   `docker run username/repository:tag`

