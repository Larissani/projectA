src = $(wildcard ../src/*.c)
include = ../include 
obj = $(patsubst %.c, %.o, $(src))
libcal = libcal.a

%.o:%.c
	gcc -c  $< -o $@  
$(libcal):$(obj)
	ar rcs $(libcal) $(obj) 
.PHONY: clean
clean :
	rm -f $(libcal) $(obj)


