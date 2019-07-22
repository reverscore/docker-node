FROM node:10.16-jessie

RUN mkdir -p /var/www \
	&& npm install -g express-generator mocha sinon should assert node-gyp nodemon eslint typescript

WORKDIR /var/www
EXPOSE 3000
CMD ["npm", "start"]
