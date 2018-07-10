# jib-docker-spring-boot-examples

https://github.com/GoogleContainerTools/jib/tree/master/jib-gradle-plugin#quickstart
https://cloudplatform.googleblog.com/2018/07/introducing-jib-build-java-docker-images-better.html
http://siosio.hatenablog.com/entry/2018/07/10/081158

## how to try it?

### Building docker image

    ./gradlew jibDockerBuild

And check it.

    $ docker images
    REPOSITORY                                      TAG                 IMAGE ID            CREATED             SIZE
    tokuhirom/jib-demo-app                          latest              6040d478fea6        292 years ago       134MB

And run docker container.

    docker run -p 8080:8080/tcp  tokuhirom/jib-demo-app

And access to http://localhost:8080/

