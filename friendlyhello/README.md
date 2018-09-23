## Build the app

<code>docker build -t friendlyhello .</code>

## To find the built image

<code>docker image ls</code>

## Run the app

Run the app, mapping your machine’s port 4000 to the container’s published port 80 using <code>-p</code>:

<code>docker run -p 4000:80 friendlyhello</code>

## To run the app in the background, in detached mode

<code>docker run -d -p 4000:80 friendlyhello</code>

## References

https://docs.docker.com/get-started/part2/w
