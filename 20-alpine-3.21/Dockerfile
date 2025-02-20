FROM node:20.18-alpine3.21

RUN apk add --no-cache --update python3 make gcc g++ git curl expat && \
	rm -rf /tmp/* /var/cache/apk/* /root/.npm /root/.node-gyp ; mkdir -p /var/www ; \
	npm install -g express-generator mocha sinon should assert node-gyp nodemon eslint typescript

WORKDIR /var/www
EXPOSE 3000
CMD ["npm", "start"]
