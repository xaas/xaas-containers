FROM ubuntu
MAINTAINER cm 2014-03-07_7

# Install vsftp
RUN apt-get update -q
RUN apt-get install -y vsftpd 

RUN mkdir -p /var/run/vsftpd/empty

# Expose ports.
EXPOSE 21

ENTRYPOINT ["vsftpd"]
