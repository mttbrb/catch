INC=-I/work/cpp/catch

CXX=clang++
CXXFLAGS=-g -std=c++11 -Wall -pedantic $(INC)
BIN=Factorial

SRC=$(wildcard *.cpp)
OBJ=$(SRC:%.cpp=%.o)

all: $(OBJ)
	$(CXX) -o $(BIN) $^

%.o: %.c
	$(CXX) $@ -c $<

clean:
	rm -f *.o
	rm $(BIN)
