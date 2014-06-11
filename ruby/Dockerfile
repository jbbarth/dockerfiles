FROM debian:wheezy

MAINTAINER Jean-Baptiste BARTH <jeanbaptiste.barth@gmail.com>

ENV DEBIAN_FRONTEND noninteractive

#prerequisites
RUN apt-get update # 2013-06-11
RUN apt-get install -y procps curl

#rvm
RUN curl -sSL https://get.rvm.io | bash -s stable
RUN bash -c "source /etc/profile.d/rvm.sh && rvm install 2.0.0-p481"
RUN bash -c "source /etc/profile.d/rvm.sh && rvm use --default 2.0.0-p481"

ENV PATH /usr/local/rvm/gems/ruby-2.0.0-p481/bin:/usr/local/rvm/gems/ruby-2.0.0-p481@global/bin:/usr/local/rvm/rubies/ruby-2.0.0-p481/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/local/rvm/bin
