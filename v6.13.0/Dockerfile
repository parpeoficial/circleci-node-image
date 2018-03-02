FROM circleci/node:6.13.0

USER root

# Add Repository
RUN sudo echo "deb http://ftp.debian.org/debian jessie-backports main" >> /etc/apt/sources.list
RUN sudo apt-get update && apt-get install -y --no-install-recommends apt-utils

# Install Command-line JSON processor (JQ)
RUN apt-get install -y jq=1.5+dfsg-1.3~bpo8+1
RUN jq --version

# Install Python
RUN apt-get install -y python