FROM openjdk:12.0.1-jdk-oraclelinux7

ADD kafdrop.sh /
ADD kafdrop*tar.gz /

RUN yum install yum-plugin-security -y
RUN yum --security update-minimal -y

RUN chmod +x /kafdrop.sh

ENTRYPOINT ["/kafdrop.sh"]
