FROM skc-centos7-base:latest
MAINTAINER Stephen K Conklin <stephen@thinkedg.com>

# update and clean
RUN yum update -y && \
    yum clean all

RUN yum install -y http://yum.puppetlabs.com/puppetlabs-release-pc1-el-7.noarch.rpm && \
    yum repolist

RUN yum install -y puppet-agent


RUN export PATH=$PATH:/opt/puppetlabs/bin >> /root/.bash_profile


CMD /usr/sbin/init
