docker-snort
============

Snort in a Docker Container

Install
============

- Install Docker - http://docs.docker.io/en/latest/installation/ubuntulinux/
- On the host: sudo apt-get install build-essential checkinstall autoconf bison flex libpcap-dev libpcre3-dev zlib1g-dev libnuma-dev libtool
- Clone the repo
- Go to the debs directory and run run.sh to build the deb requirements
- modprobe pf_ring and/or ensure it starts on startup
- If everything works out correctly, you should be able to run the test.sh script and run snort using the /run.sh file

Todo
====

- Need to check that the kernel modules is already installed on the host, if not build it
- Should probably have a switch to only make the debs so it can be installed on other hosts
- Check for any other host based requirements and document them
- Get configs out, and actually run snort as a service
- Ensure signatures actually update

Tip Jar: https://gist.github.com/coolacid/9537573