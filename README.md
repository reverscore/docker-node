# Node.js running on Alpine

Tags available:

- ubuntu 
- alpine latest

All images have the modifications needed to run applications on /var/www

To build

    $ docker build --tag=rever/node:latest .
    $ docker build --tag=rever/node:alpine .
    $ docker build --tag=rever/node:ubuntu .

Running
The image will run npm start on /var/www, whatever you throw at it it will run

