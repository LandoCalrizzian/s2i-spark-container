FROM registry.access.redhat.com/ubi7/python-36

USER root
RUN yum -y install java-1.8.0-openjdk maven &&\
    yum clean all
USER 1001
RUN pip install pyspark==2.2.1
RUN fix-permissions /opt/app-root
