# Start from the ubuntu image
FROM ubuntu:22.04

# Use /usr/src/app as our workdir.
WORKDIR /usr/src/app

# Install curl
RUN <<EOF 
apt-get update -q
apt-get install -q -y curl
EOF

# Copy script to working directory
COPY ./script.sh .

# make the script executable
RUN chmod +x script.sh

# When running docker
ENTRYPOINT ["./script.sh"]

