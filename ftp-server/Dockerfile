FROM ubuntu
MAINTAINER cm 2014-03-10_4

# Install vsftp
RUN apt-get update -q
RUN apt-get install -y vsftpd 
# Create dummy folder, needed by vsftpd
RUN mkdir -p /var/run/vsftpd/empty

# Add configuration file
ADD vsftpd.conf /etc/vsftpd.conf

# Expose ports.
EXPOSE 21

# ENTRYPOINT ["vsftpd"]
