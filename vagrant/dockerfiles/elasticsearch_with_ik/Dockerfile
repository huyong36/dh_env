# Base dockerfile/elasticsearch
FROM dockerfile/elasticsearch
MAINTAINER huyong36 <joyhu8023danny@gmail.com>
#install ik
RUN cd /opt/elasticsearch/lib;wget https://github.com/medcl/elasticsearch-rtf/blob/master/elasticsearch/plugins/analysis-ik/elasticsearch-analysis-ik-1.2.5.jar?raw=true -O elasticsearch-analysis-ik-1.2.5.jar --no-check-certificate;wget https://github.com/medcl/elasticsearch-rtf/blob/master/elasticsearch/plugins/analysis-pinyin/elasticsearch-analysis-pinyin-1.2.1.jar?raw=true -O elasticsearch-analysis-pinyin-1.2.1.jar --no-check-certificate;wget https://github.com/medcl/elasticsearch-rtf/blob/master/elasticsearch/plugins/analysis-pinyin/pinyin4j-2.5.0.jar?raw=true -O pinyin4j-2.5.0.jar --no-check-certificate

RUN cd /opt/elasticsearch/config;wget http://github.com/downloads/medcl/elasticsearch-analysis-ik/ik.zip --no-check-certificate; unzip ik.zip; rm ik.zip;wget https://github.com/huyong36/dh_env/blob/master/vagrant/dockerfiles/elasticsearch_with_ik/elasticsearch.yml?raw=true -O elasticsearch.yml

#RUN elasticsearch -Des.index.analysis.analyzer.ik.type="ik"
