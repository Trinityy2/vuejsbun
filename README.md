# vuejsbun
Bun is a new Javascript compiler/Typescript transpiler designed with speed in mind.
This repo contains example templates to use bun to run a dockerised VueJS web app.

## Instructions
### From scratch
1. Use bun to create a vuejs app using vite by running `bun create vite <app_name>`
2. Navigate into your app using `cd <app_name>` and run `bun install`
3. Copy BOTH Dockerfile and .dockerignore from this repo into folder*
4. Build docker image using `docker build . --tag vuejsbun`
5. Create and run docker container using `docker run vuejsbun --publish 5050:5050`

* If you want to create one for a development, use `Dockerfile.development` instead

## Todo
1. Create dockerfile for production server
2. Add command for mounting volumes for development