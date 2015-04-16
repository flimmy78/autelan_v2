
default:	build

clean:
	rm -rf Makefile objs

build:
	$(MAKE) -f objs/Makefile
	$(MAKE) -f objs/Makefile manpage

install:
	$(MAKE) -f objs/Makefile install

upgrade:
	/home/hisisdk/histb_v2/autelan/rootfs/nginx-1.7.12/../../release/usr/sbin/ -t

	kill -USR2 `cat /tmp/pid/nginx/nginx.pid`
	sleep 1
	test -f /tmp/pid/nginx/nginx.pid.oldbin

	kill -QUIT `cat /tmp/pid/nginx/nginx.pid.oldbin`
