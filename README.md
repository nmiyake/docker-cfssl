CFSSL Docker Image
==================
Provides a base Docker image that contains common services and utilities useful for CFSSL usage. It
is based on the [CentOS 6 image](https://hub.docker.com/_/centos/) and contains the following
additions:

  * wget
  * unzip
  * netcat
  * openssl
  * rubygems
  * [dumb-init](https://github.com/Yelp/dumb-init)
  * [jq](https://github.com/stedolan/jq)
  * [cfssl](https://github.com/cloudflare/cfssl)
