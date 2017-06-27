FROM ubuntu:latest

RUN apt-get update && apt-get install -y tar gzip bzip2 \
  wget \
  build-essential 
  
RUN  wget https://github.com/alexdobin/STAR/archive/2.5.3a.tar.gz \
  && tar -zxvf 2.5.3a.tar.gz \
  && rm -r 2.5.3a.tar.gz 


CMD ["/bin/bash"]
