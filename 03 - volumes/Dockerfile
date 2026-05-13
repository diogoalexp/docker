FROM node:14

ARG DEFAULT_PORT=80

WORKDIR /app

COPY package.json .

RUN npm install

#you can remove it if you use Bind Mount (used only when in a development machine to hotreload)
# -v "C:\workspace\study\Docker\03 - volumes\1 - data-volumes:/app:ro"
COPY . .

ENV PORT=$DEFAULT_PORT

EXPOSE $PORT

#anonymous volume will be alive as long with the container
# VOLUME [ "/app/feedback" ]

#name volumes will persists even if you delete the container
#run the container with "-v feedback:/app/feedback" flag with the name:path param

# commented here because the command is making the app readonly, so we need to define this volume in the command
# docker run -p 3000:80 -d --rm --name feedback-app -v feedback:/app/feedback -v "C:\workspace\study\Docker\03 - volumes\1 - data-volumes:/app:ro" -v /app/temp -v /app/node_modules feedback-node:volumes
# VOLUME [ "/app/temp" ]

CMD ["npm", "start"]