
RM = rm -f
CC = gcc
CFLAGS = -Wall -g
INCLUDES = 
LDFLAGS = -lglut -lGL -lGLU -lm
LDPATH =

SOURCES = $(shell ls *.c)
PROGS = $(subst .c,,$(SOURCES))
#PROGS = $(SOURCES:%.cpp=%)

all: $(PROGS)
	@echo "PROGS = $(PROGS)" 

clean:
	$(RM) $(PROGS)

%: %.c
	$(CC) -o $@ $(CFLAGS) $(INCLUDES) $^ $(LDFLAGS) $(LDPATH)
