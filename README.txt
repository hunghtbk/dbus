Ubuntu 16.04(best) or 18.04

1. https://github.com/GENIVI/capicxx-dbus-tools/wiki/CommonAPI-C---D-Bus-in-10-minutes
2. https://github.com/GENIVI/capicxx-someip-tools/wiki/CommonAPI-C---SomeIP-in-10-minutes

3. Install gcc-4.9:
	1.su to root, and modify /etc/apt/sources.list by adding

	deb http://dk.archive.ubuntu.com/ubuntu/ xenial main
	deb http://dk.archive.ubuntu.com/ubuntu/ xenial universe
	2.update the source by
	
	sudo apt-get update
	3.install
	
	sudo apt-get install gcc-4.9
	
4. Apply version 4.9 for gcc and g++
	
	sudo su
	rm /usr/bin/gcc
	rm /usr/bin/g++
	
	ln -s /usr/bin/gcc-4.9 /usr/bin/gcc
	ln -s /usr/bin/g++-4.9 /usr/bin/g++
	
5. Install boost
	sudo apt-get install libboost.1.58-dev
	sudo apt install libboost-system-dev libboost-thread-dev libboost-program-options-dev libboost-test-dev
	sudo apt -y install libboost-filesystem-dev
