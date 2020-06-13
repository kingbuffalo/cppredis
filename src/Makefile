CC=g++
CFLAGS= -std=c++14 -I. 
OBJFLAG=-lpthread
SRCS=$(wildcard *.cpp)
OBJ = ${patsubst %.cpp,%.o,$(SRCS)}


%.o: %.cpp
	$(CC) -c -g $< $(CFLAGS)

main:$(OBJ)
	$(CC) -g -o $@ $(OBJ) $(OBJFLAG)

.PHONY: clean
clean:
	rm -rf main *.o
