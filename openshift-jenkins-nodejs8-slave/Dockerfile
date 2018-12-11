FROM openshift/jenkins-slave-base-centos7
 
# `node-gyp rebuild` requires python, make & g++
RUN yum update -y
RUN yum install -y vim g++ make git rh-python36
RUN yum clean all
RUN python -v
 
RUN curl --silent --location https://rpm.nodesource.com/setup_8.x | bash -
RUN yum -y install nodejs && yum clean all -y
RUN node -v
RUN npm -v
