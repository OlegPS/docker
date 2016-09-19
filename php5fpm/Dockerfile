
FROM debian:jessie
MAINTAINER Oleg Selin <oleg.selin@gmail.com>
RUN apt-get update \
	&& apt-get install -y php5-fpm php5-mysql \
	&& echo "/etc/php5/mods-available/mysqli.ini" >> /etc/php5/cli/php.ini
CMD ["/usr/sbin/php5-fpm", "--nodaemonize", "--fpm-config", "/etc/php5/fpm/php-fpm.conf"]
