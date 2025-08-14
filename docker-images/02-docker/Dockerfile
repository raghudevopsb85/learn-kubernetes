FROM          redhat/ubi9
ADD           sample.txt /opt/sample.txt
ARG           URL
RUN           echo $URL
ENV           URL1=google.com
USER          bin
WORKDIR       /etc
#ENTRYPOINT    ["id"]
RUN           dnf install iputils-20210202-11.el9_6.1.x86_64 -y
ENTRYPOINT    ["ping", "-c", "3"]
