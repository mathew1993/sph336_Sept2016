#      Makefile
#      Created on: Nov 12, 2016
#      Author: Mathew

GTKWAVE := $(shell which gtkwave)

all: decoder

decoder:prerequisites
	@echo 'building file $(@F)'
	$(CXX) -I/usr/local/systemc-2.3.1/include -O0 -g3 -Wall -c decoder_2by4.cc
	$(CXX) -L/usr/local/systemc-2.3.1/lib-linux64 -o "gotv2" decoder_2by4.o -lsystemc
	./gotv2
	gtkwave -c 4 timing_diagram.vcd

prerequisites: 
ifneq "$(GTKWAVE)" "/usr/bin/gtkwave"
	@echo 'installing gtkwave, please be patient'
	sudo apt-get install -y gtkwave
endif
.PHONY: decoder
