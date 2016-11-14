FROM ubuntu

MAINTAINER genDevOps

# Add binaries
ADD artifacts/* /usr/bin

# Ports
EXPOSE 80

# Run
CMD ["api", "--listen", ":80", "--db", "10.1.21.21:27000"]
