botox
=====

Refer to https://code.google.com/p/botox/source/browse/trunk/src

DESCRIPTION
===========

	Botox is a simple tool designed to make it easier to intercept and debug
	short-lived processes, such as CGI scripts. It can detect when the desired
	process has been loaded into memory, pause the process execution and run
	a specified command (by default, it invokes gdbserver).

	Botox polls the /proc directory waiting for the target process to be instantiated. 
	Once the target process is detected, Botox will pause the process, then execute 
	the specified command (typically gdb/gdbserver).

USAGE
=====

		$sudo apt-get install gcc automake autoconf libtool make
	
	Edit conf.h with the desired command to execute, then:

		$ ./configure && make
