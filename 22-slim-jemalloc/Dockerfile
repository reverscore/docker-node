FROM node:22.14.0-slim

RUN apt-get update && apt-get install -y python3 make gcc g++ git curl expat && \
	rm -rf /tmp/* /var/cache/apk/* /root/.npm /root/.node-gyp ; mkdir -p /var/www ;

# install jemalloc and preload it so that all applications use it
RUN apt-get install -y libjemalloc-dev
RUN touch /etc/ld.so.preload
RUN find / -name "*jemalloc*.so" >  /etc/ld.so.preload

RUN npm install -g express-generator mocha sinon should assert node-gyp nodemon eslint typescript

WORKDIR /var/www
EXPOSE 3000
CMD ["npm", "start"]
