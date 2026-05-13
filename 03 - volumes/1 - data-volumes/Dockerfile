FROM node:14

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

#anonymous volume will be alive as long with the container
# VOLUME [ "/app/feedback" ]

#name volumes will persists even if you delete the container
#run the container with "-v feedback:/app/feedback" flag with the name:path param

CMD ["npm", "start"]