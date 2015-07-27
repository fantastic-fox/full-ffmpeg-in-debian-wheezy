full-ffmpeg-in-debian-wheezy
============================

Build, create .deb &amp; install full ffmpeg in debian wheezy - optionally using docker

	git clone git://github.com/fantastic-fox/full-ffmpeg-in-debian-wheezy.git
	cd full-ffmpeg-in-debian-wheezy/
	docker build -t="ffmpeg-build-debian" .
	
.deb file location:

	~/ffmpeg_sources/ffmpeg/ffmpeg_2.7.2-1_amd64.deb

To install:

	# install ffmpeg
	dpkg --install ffmpeg_2.7.2-1_amd64.deb
	# install missing dependencies
	apt-get update
	apt-get -f install