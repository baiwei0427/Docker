To build the helloworld image:

```
$ docker build -t helloworld:latest .
``` 

To see the built helloworld image:


``` 
$ docker image ls
REPOSITORY              TAG                 IMAGE ID            CREATED             SIZE
helloworld              latest              ea8cbfc07b6b        15 minutes ago      13.6MB
``` 

Note that the image size is very small as we use [multi-stage build](https://docs.docker.com/develop/develop-images/multistage-build/).

To run the image:
```
$ docker run --rm -ti helloworld
Hello World
```
