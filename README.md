docker-wso2as
=============

Docker Image for WSO2 Application Server(AS).

The dockerfile will:

* Copy `AS 4.9.0 zip` to /otp from Packages directory.
* Unzip the AS 4.9.0 ZIP.
* Expose the container port `9443`.
* Set the ESB `wso2server.sh` start-up script as the container start-up command.

### Usage
* To pull: `docker pull anitech/wso2-as`
* To build: `docker build -t your_image_name github.com/tapas4java/docker-wso2as`
* To run: `docker run --rm --name your_container_name -p 9443:9444 your_image_name`
* To access ESB web admin console, navigate to `https://localhost:9444`