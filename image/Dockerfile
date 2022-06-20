FROM ubuntu:latest

RUN apt-get update
RUN apt-get install python3 -y

RUN apt install software-properties-common -y
RUN add-apt-repository --yes --update ppa:ansible/ansible

RUN apt-get install ansible -y

RUN apt-get install git -y
RUN git clone https://github.com/IvanciniGT/cursoITNowAnsible /repo_empresa
ENV ANSIBLE_ROLES_PATH=/repo_empresa/roles

RUN mkdir -p /root/.ssh
RUN touch /root/.ssh/known-hosts

CMD ["sh", "-c", "tail -f /dev/null"]


