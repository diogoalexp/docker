FROM node

WORKDIR /app

#. root directory
#./ work directory
# /app specific directory

# {outside path} {inside container path}
COPY . ./

RUN npm install

#port that will be used in the machine
EXPOSE 80

#run starts when the container is created
#cmd starts when the containers is started

# CMD node server.js
CMD ["node", "server.js"]

