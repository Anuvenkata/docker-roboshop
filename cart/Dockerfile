FROM node:20
WORKDIR /opt/server
EXPOSE 8080
COPY package.json .
COPY *.js .
RUN npm install
ENV REDIS-HOST="redis" \
    CATAlOGUE-HOST="catalogue" \
    CATALOGUE-PORT="8080"
CMD ["node" , "server.js"]