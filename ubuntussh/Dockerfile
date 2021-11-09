FROM ubuntu:20.04

RUN apt update && apt install  openssh-server sudo -y

RUN  echo 'root:builder' | chpasswd

RUN service ssh start

EXPOSE 22

CMD ["/usr/sbin/sshd","-D"]
