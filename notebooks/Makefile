NOTEBOOKS = $(shell git ls-files [0-9]*)

all: style

include Makefile.style

include Makefile.norm

########## BOOK
book:
	jupyter-book build .



.PHONY: all norm style book
