FROM node:18.17.0-alpine
WORKDIR /var/www/html/elpis
# COPY /src_v2 ./

RUN npm install pm2 -g && apk add gcc
ENV NODE_ENV production
EXPOSE 3000
CMD ["pm2-runtime", "dist/server/index.js","-i"," max" ]