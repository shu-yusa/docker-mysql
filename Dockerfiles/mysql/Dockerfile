FROM mysql:5.7
MAINTAINER yusa
ADD mysqld.cnf /etc/mysql/mysql.conf.d/mysqld.cnf

RUN apt-get update
RUN apt-get install -y vim
ADD vimrc /root/.vimrc
RUN echo "alias ls='ls -hp'" >> /root/.bashrc
RUN echo "alias ll='ls -l'" >> /root/.bashrc
RUN echo "alias la='ls -la'" >> /root/.bashrc
RUN echo "alias vi='vim'" >> /root/.bashrc

EXPOSE 3306
