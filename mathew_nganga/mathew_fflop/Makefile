

GTKWAVE := $(shell which gtkwave)
triangle:=flipflop

all: flipflop

flipflop:prerequisites
	@echo 'building file $(@F)'
	$(CXX) -I/usr/local/systemc-2.3.1/include -O0 -g3 -Wall -c main.cc
	$(CXX) -L/usr/local/systemc-2.3.1/lib-linux -o "flip" main.o -lsystemc
	./$(2BY4)
	gtkwave -c 4 timingF_diagram.vcd

prerequisites: 
ifneq "$(GTKWAVE)" "/usr/bin/gtkwave"
	@echo 'installing gtkwave, please be patient'
	sudo apt-get install -y gtkwave
endif

clean:
	rm *.out *.o *.vcd

.PHONY: flipflop
