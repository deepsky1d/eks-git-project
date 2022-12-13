FROM node:14.17

WORKDIR /home/app

RUN npm install pm2 -g

COPY package*.json /home/app/

RUN npm install 

COPY . /home/app/

EXPOSE 5000

CMD ["pm2-runtime", "start", "/home/app/index.js"]
