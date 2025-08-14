FROM          redhat/ubi9
ADD           sample.txt /opt/sample.txt
ARG           URL
RUN           echo $URL
ENV           URL1=google.com
USER          bin
WORKDIR       /etc
#ENTRYPOINT    ["id"]
RUN           dnf install ping -y
ENTRYPOINT    ["ping", "-c", "3"]
