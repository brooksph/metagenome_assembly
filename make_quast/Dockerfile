#This Dockerfile is for QUAST-4.0
FROM ubuntu:14.04
RUN apt-get update 
# Dependencies
RUN apt-get install -y g++                           make                           wget                           python                           python-matplotlib                           zlib1g-dev                           cmake                           openjdk-6-jdk                           curl                           libboost-all-dev \   
                          libncurses5-dev
                          
# Clone Quast git repo
RUN wget -O- https://github.com/ablab/quast/archive/release_4.0.tar.gz | tar zxvf -
RUN chmod +x /quast-release_4.0/quast.py

WORKDIR /quast-release_4.0/libs/samtools
RUN ./configure && make && make install

ENTRYPOINT ["/quast-release_4.0/quast.py"]
CMD ["-h"]

#To test docker run quast_ctr -h
#To link data 

