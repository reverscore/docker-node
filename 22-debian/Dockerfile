FROM node:22.23.4-bookworm-slim

RUN apt-get update && apt-get install -y python3 make gcc g++ git curl expat && \
	rm -rf /tmp/* /var/cache/apk/* /root/.npm /root/.node-gyp ; mkdir -p /var/www ;

RUN npm install -g express-generator mocha sinon should assert node-gyp nodemon eslint typescript

WORKDIR /var/www
EXPOSE 3000
CMD ["npm", "start"]