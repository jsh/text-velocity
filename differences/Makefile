SHELL := /bin/bash
PATH += :

../bin/fd: fd
	install -D $< $@

powers-of-two:
	y=1; for x in {0..61}; do y=$((y*2)); echo $x $y; done > $@

sums-of-two:
	y=1; for x in {0..61}; do y=$((y+2)); echo $x $y; done > $@

test: powers-of-two sums-of-two
	for i in t{1,2}; do $$i; done
	
