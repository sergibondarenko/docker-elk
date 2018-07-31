# https://github.com/elastic/kibana-docker
FROM docker.elastic.co/kibana/kibana-oss:6.2.4

# Add your kibana plugins setup here
RUN kibana-plugin install https://github.com/sirensolutions/sentinl/releases/download/tag-6.2.4-pre-0/sentinl-v6.2.4.zip

USER root
RUN yum update -y && yum install -y fontconfig freetype net-tools && yum clean all

USER kibana
