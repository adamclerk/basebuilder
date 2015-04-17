# this file describes how to build tsuru go image
# to run it:
# 1 - tsuru-admin platform-add godep -d https://raw.github.com/adamclerk/basebuilder/master/godep/Dockerfile

from	ubuntu:14.04
run	apt-get update
run	apt-get install wget -y --force-yes
run	wget http://github.com/adamclerk/basebuilder/tarball/master -O basebuilder.tar.gz --no-check-certificate
run	mkdir /var/lib/tsuru
run	tar -xvf basebuilder.tar.gz -C /var/lib/tsuru --strip 1
run	cp /var/lib/tsuru/go/deploy /var/lib/tsuru
run	cp /var/lib/tsuru/go/start /var/lib/tsuru
run	/var/lib/tsuru/go/install
