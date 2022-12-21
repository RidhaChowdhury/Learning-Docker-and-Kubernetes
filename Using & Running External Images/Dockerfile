#THESE ARE INSTRUCTIONS FOR SETTING UP THE IMAGE
FROM node

WORKDIR /app
#first . indicates that docker should pull everything from the directory this Dockerfile is in
#./ copy it into the working directory of the container

COPY . /app

RUN npm install

# we want port 80 in the isolated docker container to be exposed to our local machine
EXPOSE 80

#whenever a container is created from this image node is used to run server js
#this should always be the last commnad
CMD ["node", "server.js"]