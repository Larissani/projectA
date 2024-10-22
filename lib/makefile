target = main
src = $(wildcard *.c ../src/*.c)
obj = $(patsubst %.c,%.o,$(src))
include = ../include
%.o : %.c
	gcc -c $< -o $@
libcal : $(obj)
	ar rcs libcal.a $(obj)
$(target) : libcal $(obj)
	gcc $(obj) -I$(include)  -lcal -L. -o $(target) 
.PHONY: clean
clean:
	rm -f $(obj) $(target) libcal 


