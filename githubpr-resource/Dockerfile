FROM debian

RUN apt update
RUN apt install -y python python-pip

RUN pip install pygithub

ADD assets/ /usr/local/bin/

RUN mkdir /opt/resource/
RUN ln -s /usr/local/bin/check_github_pr /opt/resource/check
RUN ln -s /usr/local/bin/check_github_pr /opt/resource/in
RUN ln -s /usr/local/bin/check_github_pr /opt/resource/out
