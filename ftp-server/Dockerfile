FROM ubuntu
MAINTAINER cm 2014-03-10_8

# Install vsftp
RUN apt-get update -q
RUN apt-get install -y vsftpd 
# Create dummy folder, needed by vsftpd
RUN mkdir -p /var/run/vsftpd/empty

# Add configuration file
ADD vsftpd.conf /etc/vsftpd.conf
RUN chown root /etc/vsftpd.conf
RUN chmod 777 /etc/vsftpd.conf

# Expose ports.
EXPOSE 20
EXPOSE 21

# ENTRYPOINT ["vsftpd"]
