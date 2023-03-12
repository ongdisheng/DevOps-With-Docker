# Start from the ubuntu image
FROM ubuntu:20.04

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# Copy the website.sh file from this location to /usr/src/app/ creating /usr/src/app/website.sh.
COPY website.sh .

# Execute a command with `/bin/sh -c` prefix.
RUN apt-get update
RUN apt-get -y install curl

# When running Docker run the command will be ./website.sh
CMD ./website.sh