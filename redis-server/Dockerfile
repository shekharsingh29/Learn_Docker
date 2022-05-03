# Mention the base image
FROM alpine


# Issue the command to install the package for dependency
RUN apk add --update redis
RUN apk add --update gcc

# Tell the container what to do
CMD ["redis-server"]



