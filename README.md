docker-wso2as
=============

Docker Image for WSO2 Application Server(AS).

The dockerfile will:

* Copy `AS 5.3.0 zip` to `/opt` from Packages directory.
* Unzip the `AS 5.3.0 ZIP`.
* Expose the container port `9444`.
* Set the AS `wso2server.sh` start-up script as the container start-up command.

### Usage
* To pull: `docker pull anitech/wso2-as`
* To build: `docker build -t your_image_name github.com/tapas4java/docker-wso2as`
* To run: `docker run --name your_container_name -p 9444:9443 your_image_name`
* To access Application Server web admin console, navigate to `https://localhost:9444/carbon`