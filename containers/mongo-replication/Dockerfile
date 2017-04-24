FROM ubuntu
RUN apt-get update -y && apt-get upgrade -y
RUN apt-get install -y wget \
    && wget http://downloads-distro.mongodb.org/repo/debian-sysvinit/dists/dist/10gen/binary-amd64/mongodb-10gen_2.0.5_amd64.deb -O /usr/local/src/mongodb-10gen.deb \
    && dpkg -i /usr/local/src/mongodb-10gen.deb
