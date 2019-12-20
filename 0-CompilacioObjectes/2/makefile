# Llista d'objectes
OBJS := hello.o hello2.o

all: prog

clean: # netejem objectes
	rm -rf *.o

ultraclean: clean  # netejem objectes i programa
	rm -rf prog

#####

prog: main.cpp $(OBJS)  # compilem programa (amb objectes)
	g++ -std=c++11 -o prog main.cpp $(OBJS)

hello2.o: hello2.cpp hello.hpp # compilació customitzada de hello2.o, donat que el seu .hpp es hello.hpp en lloc de hello2.hpp
	g++ -std=c++11 -c -o $@ $<

#####

%.o: %.cpp %.hpp # compilació d'un objecte genèrica, on es complia <nom>.cpp i resulta <nom>.o
	g++ -std=c++11 -c -o $@ $<
