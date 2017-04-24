# aleph-docker-tikaserver

Tika Server for use with Aleph

This repo contains the Dockerfile to create a docker image that contains the latest Ubuntu running the Apache Tika 1.15 Server on Port 9998 using Java 8.


## Usage

First you need to pull down the build from Dockerhub, which can be done by invoking:

    docker pull maquchizi/aleph-docker-tikaserver

Then to run the container, execute the following command:

    docker run -d -p 9998 maquchizi/aleph-docker-tikaserver

## Building

To build the image from scratch, simply invoke:

    docker build -t 'docker-tikaserver' .
   
You can then use the following command (using the name you allocated in the build command as part of -t option):

    docker run -d -p 9998 docker-tikaserver
    
## More

For more info on Apache Tika Server, go to the [Apache Tika Server documentation](http://wiki.apache.org/tika/TikaJAXRS).
