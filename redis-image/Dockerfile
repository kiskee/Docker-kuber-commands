# use an existing docker image as a base
FROM alpine

# download the latest version of redis and install a dependency
RUN apk add --update redis
RUN apk add --update gcc


# tell the image what to do when it starts as a container
CMD ["redis-server"]


## to run this just put docker build .
## then it will give us an image id and put docker run <image id>