all: output messagelib.a

output: main.o messagelib.a
	g++ main.o messagelib.a -o output

main.o: main.cpp
	g++ -c main.cpp

message.o: message.cpp message.h
	g++ -c message.cpp

messagelib.a: message.o
	ar -rcs messagelib.a message.o

clean:
	rm -rf *.o
