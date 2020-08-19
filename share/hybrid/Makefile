#!/usr/bin/make -f

PROGRAM = gpu-manager
PROGRAM_FILES = gpu-manager.c
CC = gcc
CFLAGS =-g -Wall $(shell pkg-config --cflags --libs pciaccess libdrm libkmod json-c) -lz

all: build

build:
	$(CC) -o $(PROGRAM) $(PROGRAM_FILES) $(CFLAGS)

clean:
	@rm -f $(PROGRAM)
