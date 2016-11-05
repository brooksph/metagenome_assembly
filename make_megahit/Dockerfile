FROM ubuntu:14.04
RUN apt-get update
RUN apt-get install -y g++ make git zlib1g-dev python
RUN git clone https://github.com/voutcn/megahit.git /home/megahit
RUN cd /home/megahit && make
CMD /mydata/do-assemble.sh
