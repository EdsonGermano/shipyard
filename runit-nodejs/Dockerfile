FROM socrata/runit
MAINTAINER Socrata <sysadmin@socrata.com>

RUN apt-get -y update && apt-get install -y libyajl2

RUN DEBIAN_FRONTEND=noninteractive apt-get update && apt-get -y install nodejs npm
RUN npm install -g n
RUN n 6.9.1

# LABEL must be last for proper base image discoverability
LABEL repository.socrata/nodejs=""
