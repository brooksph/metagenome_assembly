FROM ubuntu:14.04
RUN apt-get update && apt-get install git python-setuptools python-pip -y            
RUN git clone https://github.com/relipmoc/skewer.git
RUN cd skewer
RUN pip install skewer
