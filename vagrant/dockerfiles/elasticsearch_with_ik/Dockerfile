# Base dockerfile/elasticsearch
FROM dockerfile/elasticsearch
MAINTAINER huyong36 <joyhu8023danny@gmail.com>
#install ik
RUN cd /opt/elasticsearch/lib; wget https://github.com/medcl/elasticsearch-rtf/blob/master/elasticsearch/plugins/analysis-ik/elasticsearch-analysis-ik-1.2.5.jar?raw=true -O elasticsearch-analysis-ik-1.2.5.jar --no-check-certificate

RUN cd /opt/elasticsearch/config; wget http://github.com/downloads/medcl/elasticsearch-analysis-ik/ik.zip --no-check-certificate; unzip ik.zip; rm ik.zip
RUN cd /opt/elasticsearch/config; wget  https://github.com/medcl/elasticsearch-rtf/blob/master/elasticsearch/config/elasticsearch.yml?raw=true -O elasticsearch.yml
#RUN elasticsearch -f -Des.index.analysis.analyzer.ik.type="ik"
