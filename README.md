# Node.js running on Alpine

Tags available:

- 10-jessie 
- alpine latest

All images have the modifications needed to run applications on /var/www

To build

    $ docker build --tag=rever/node .
    $ docker build --tag=rever/node-ubuntu

Running
The image will run npm start on /var/www, whatever you throw at it it will run

