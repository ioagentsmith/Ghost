#FROM ghost
FROM bennetimo/ghost-wait-mysql
MAINTAINER Christoff Smith <christoff@ioagentsmith.co.za>


# Wait for SQL to start
ENV MYSQL_HOST=mysql
ENV MYSQL_PORT=3306
ENV WAIT_LOOPS=10
ENV WAIT_SLEEP=2

# Create required volumes
VOLUME ["/var/lib/mysql", "/var/lib/ghost"]

# Run Ghost
#ENV NODE_ENV production
ENTRYPOINT ["/bin/bash"] 
