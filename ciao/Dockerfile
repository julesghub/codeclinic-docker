FROM ubuntu:22.10

# setup environment
RUN apt-get update
RUN apt-get install -y python3-pip
#RUN rm -rf /var/lib/apt/lists/*

# get python packages
RUN pip install art

# setup /workspace in container
RUN mkdir -p /workspace
# move files into contain
COPY . /workspace

# execution command
CMD ["python3", "/workspace/ciao.py"]
