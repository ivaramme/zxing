#### Introduction 

Web application artefact that implements the old Google Chart Service API. More information: https://github.com/zxing/zxing/wiki/Chart-Server-Parameters

Included is a basic Dockerfile that packs the generated WAR file and adds it to Tomcat server instance version 8 as its ROOT application (as this is how the app was coded)

#### Instructions:

Create WAR file:  `mvn clean -U package`

Build Docker image: `docker build -t zxing .`

Run Docker container: `docker run -it --rm -p8080:8080 zxing`

To test locally: `http://localhost:8080/w/chart?cht=qr&chs=200x200&chld=H%7C6&choe=UTF-8&chl=Hello+World`
