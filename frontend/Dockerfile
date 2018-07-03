# FRONTEND TOOLSET
# Version: 1.08
# https://github.com/jasonamartin/docker-files/frontend-toolset/
# BUILD IMAGE
# docker build -t jasonamartin/frontend:1.08
# RUN COMMANDS (removed container once exited)
# Example: This runs npm i on current directory
# docker run -it --rm -p 3000:3000 -v "$PWD":/app  jasonamartin/frontend:1.08 node -v
FROM node:10

LABEL maintainer="jason.martin@jasonamartin.com"

RUN npm install -g gulp-cli grunt gulp bower jest eslint webpack webpack-cli webpack-dev-server

CMD ["/bin/bash"]

EXPOSE 80 3000

VOLUME ["/app"]

WORKDIR ["/app"]
