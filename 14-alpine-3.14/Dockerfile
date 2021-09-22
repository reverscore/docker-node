FROM node:14.17.0-alpine3.14

RUN apk add --no-cache make gcc g++ git && \
	rm -rf /tmp/* /var/cache/apk/* /root/.npm /root/.node-gyp ; mkdir -p /var/www ; \
	npm install -g express-generator mocha sinon should assert node-gyp nodemon eslint typescript

WORKDIR /var/www
EXPOSE 3000
CMD ["npm", "start"]
