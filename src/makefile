target = main
include = ../include

libcal = ../lib/


$(target) : $(include)  $(libcal)
	gcc -o $@ ../main.c -I$(include) -lcal -L$(libcal) 
.PHONY : clean
clean:
	rm -f $(target)

