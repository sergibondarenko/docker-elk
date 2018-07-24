# https://github.com/elastic/kibana-docker
FROM docker.elastic.co/kibana/kibana-oss:6.2.4

# Add your kibana plugins setup here
RUN kibana-plugin install https://github.com/sirensolutions/sentinl/releases/download/tag-6.2.4-pre-0/sentinl-v6.2.4-3.zip
#RUN kibana-plugin install https://github.com/sirensolutions/sentinl/releases/download/tag-6.2.4-pre-0/sentinl-v6.2.4-puppeteer-0.zip

#USER root
#RUN yum -y install libX11 libXcomposite libXcursor libXdamage libXext libXi libXtst cups-libs libXScrnSaver libXrandr alsa-lib pango atk at-spi2-atk gtk3

USER root
RUN yum -y install fontconfig freetype freetype-devel fontconfig-devel libstdc++
ENV PATH="/usr/share/kibana/node/bin:${PATH}"
