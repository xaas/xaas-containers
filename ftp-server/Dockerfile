FROM ubuntu
MAINTAINER cm 2014-03-07_4

# Install vsftp
RUN apt-get update -q
RUN apt-get install -y vsftpd 

# Expose ports.
EXPOSE 21

ENTRYPOINT ["vsftpd &"]
