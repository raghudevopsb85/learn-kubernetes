FROM          redhat/ubi9
ADD           sample.txt /opt/sample.txt
ARG           URL
RUN           echo $URL
ENV           URL1=google.com
RUN           dnf install iputils-20210202-11.el9_6.1.x86_64 -y
USER          bin
WORKDIR       /etc
#ENTRYPOINT    ["id"]
ENTRYPOINT    ["ping", "-c", "3"]
CMD           ["yahoo.com"]
