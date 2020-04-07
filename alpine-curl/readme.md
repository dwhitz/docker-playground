
# Simple curl image with docker

Use curl with a docker container in order to does not invoke curl manually each time
    e.g. docker run `<image-name>` curl www.google.com

## 1. Update and add curl

    apk update && apk add curl

## 2. Set curl as entrypoint

     ENTRYPOINT ["curl"]

## 3. Test our image

    docker run dwhitz/alpine-curl www.google.com  ==> will print the html of www.google.com

