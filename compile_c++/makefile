a.o : a.cc
	c++ -c a.cc -o a.o
b.o : a.cc
	c++ -c b.cc -o b.o
hello : a.o b.o
	c++ a.o b.o -o hello
