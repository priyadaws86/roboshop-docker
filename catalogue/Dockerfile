FROM node:20
WORKDIR /opt/server                    #opt-optional, server is the name of the folder where we are going to copy the files
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue" 
CMD ["node", "server.js"]

