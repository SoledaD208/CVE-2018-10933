# CVE-2018-10933
to test this code: 
- get vulnerable version of libssh at homepage: https://www.libssh.org/files/0.7/libssh-0.7.4.tar.xz
- uncompress and build, then go to example directory, there's a simple sshd server using libssh name: samplesshd-cb

run this simple sshd by command:
    $ samplesshd-cb 127.0.0.1 -p 2222

- run my code, output will be:
	Allocated session channel
	Allocated shell
mean that i can bypass authentication and spawn a shell without any credential 