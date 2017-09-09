
default:	build

clean:
	rm -rf Makefile objs

build:
	$(MAKE) -f objs/Makefile
	$(MAKE) -f objs/Makefile manpage

install:
	$(MAKE) -f objs/Makefile install

upgrade:
	/Users/admin/srs-csdn/trunk/objs/nginx-1.5.7/_release/sbin/nginx -t

	kill -USR2 `cat /Users/admin/srs-csdn/trunk/objs/nginx-1.5.7/_release/logs/nginx.pid`
	sleep 1
	test -f /Users/admin/srs-csdn/trunk/objs/nginx-1.5.7/_release/logs/nginx.pid.oldbin

	kill -QUIT `cat /Users/admin/srs-csdn/trunk/objs/nginx-1.5.7/_release/logs/nginx.pid.oldbin`
