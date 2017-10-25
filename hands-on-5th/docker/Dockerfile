FROM jubatus/jubatus

WORKDIR /app
ADD . /app

# apt-get
RUN apt-get -y update && \
    apt-get -y install wget git python python-pip python-dev

# pip
RUN pip install --upgrade pip
RUN pip install Cython
RUN pip install -r requirements.txt

# git clone
RUN git clone https://github.com/jubatus/events.git

# jupyter config
RUN mkdir ~/.jupyter
COPY jupyter_notebook_config.py ~/.jupyter_notebook_config.py

# export PYTHONPATH
ENV PYTHONPATH $PYTHONPATH:/app/events/hands-on-5th/python-plugin/
