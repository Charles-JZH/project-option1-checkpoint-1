FROM helaili/vuecli as builder

COPY ./client /client
WORKDIR /client
RUN npm install && apt-get install -y vim

CMD ["npm", "run", "client"]
