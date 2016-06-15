FROM centos:6

RUN yum -y update

# Tools
RUN yum install -y wget unzip nc util-linux

# openssl
RUN yum install -y openssl

# Ruby
RUN yum install -y ruby-devel rubygems gcc
RUN gem install json

# dumbinit
RUN wget -O /usr/local/bin/dumb-init https://github.com/Yelp/dumb-init/releases/download/v1.0.1/dumb-init_1.0.1_amd64
RUN chmod +x /usr/local/bin/dumb-init

# install jq
RUN wget -O /usr/local/bin/jq https://github.com/stedolan/jq/releases/download/jq-1.5/jq-linux64
RUN chmod +x /usr/local/bin/jq

# install cfssl
RUN wget -O /usr/local/bin/cfssl https://pkg.cfssl.org/R1.2/cfssl_linux-amd64
RUN chmod +x /usr/local/bin/cfssl
RUN wget -O /usr/local/bin/cfssljson https://pkg.cfssl.org/R1.2/cfssljson_linux-amd64
RUN chmod +x /usr/local/bin/cfssljson

# install etcd
RUN curl -L https://github.com/coreos/etcd/releases/download/v2.3.5/etcd-v2.3.5-linux-amd64.tar.gz -o etcd-v2.3.5-linux-amd64.tar.gz
RUN tar xzvf etcd-v2.3.5-linux-amd64.tar.gz
RUN rm etcd-v2.3.5-linux-amd64.tar.gz
RUN mv etcd-v2.3.5-linux-amd64 etcd
