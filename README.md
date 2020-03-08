libtevent-0.10.x-srpm
=====================

SRPM building tools for libtevent-0.10.x for runing Samba 4 on RHEL 6.

This tool taken from the Fedora 29 release
The set of tools need to be built and installed in the following order.

	libtalloc-2.1.x-srpm
	libtdb-1.4.x-srpm
	libldb-2.1.x-srpm
	libtevent-0.10.x-srpm

	samba-4.12.x-srpm

The "make" command will do these steps.

	make build	# Build the package on the local OS
	make all	# Use "mock" to build the packages with the local
			# samba4repo-6-x96_64 configuration, which needs.
	make install	# Actually install the RPM's in the designated repo

		Nico Kadel-Garcia <nkadel@gmail.com>
