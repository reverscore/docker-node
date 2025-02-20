FROM node:22.14.0-alpine3.21

RUN apk add --no-cache --update python3 make gcc g++ git curl expat && \
	rm -rf /tmp/* /var/cache/apk/* /root/.npm /root/.node-gyp ; mkdir -p /var/www ;

# Install a chosen NPM version
ENV NPM_VERSION=10.3.0
RUN npm install -g npm@"${NPM_VERSION}"

RUN npm install -g express-generator mocha sinon should assert node-gyp nodemon eslint typescript

WORKDIR /var/www
EXPOSE 3000
CMD ["npm", "start"]
