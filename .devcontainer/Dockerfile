FROM "mcr.microsoft.com/devcontainers/typescript-node:1-22-bookworm"
ARG APP_NAME="baseAngular"
RUN npm install -g @angular/cli
WORKDIR ../
# RUN echo < ls -l
# RUN ng new ${APP_NAME} --directory .
RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
     && apt-get -y install --no-install-recommends chromium
ENV CHROME_BIN=/usr/bin/chromium