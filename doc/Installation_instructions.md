# Installation instructions
## Server prerequisites
The server needs the following software to run our application:
- Git "to pull the docker container from the repository"
- docker/docker_compose "to run the docker container"

## Setup backend frontend
- Create a fork of the repositories [frontend](https://github.com/hs-esslingen-It-Innovationseditor-V2-0/innovationseditor_version-2_frontend) and [backend](https://github.com/hs-esslingen-It-Innovationseditor-V2-0/innovationseditor_version-2_backend)
- Edit the `.env.example` file in both repositories with your server data
- then create a dockecontainer by merging a pull_request or running the dockerfile

## Setup server
When the backend and frontend are prepared clone the setup from the [setup repository](https://github.com/hs-esslingen-It-Innovationseditor-V2-0/itinno-server_setup) into the server
- edit the `.env.example` file to your server URL
- edit the `docker-compose-yaml` file to set your unique usernames and **save** passwords for the application
- don't forget to provide an email for the `#Let's Encrypt configuration`
- edit the paths of the `image` from frontend and backend, to the `.jar file` your build with the dockerfile.
- create the dockernetwork with:
```sh
docker network create traefik 
```


## Run the application
When the setup is done:
- load your server images with:
```sh
docker compose pull
```
- start you application:
```sh
docker compose up -d
```
When first loading the images the server needs a few minutes to do so.
## Misc
- show the server logs with 
```sh
docker compose logs
```
- stop the server with
```sh
docker compose down
```