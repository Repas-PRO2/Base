# Llista d'objectes
OBJS := hello.o

all: prog

clean: # netejem objectes
	rm -rf *.o

ultraclean: clean  # netejem objectes i programa
	rm -rf prog

#####

prog: main.cpp $(OBJS)  # compilem programa (amb objectes)
	g++ -std=c++11 -o prog main.cpp $(OBJS)

#####

%.o: %.cpp %.hpp # compilació d'un objecte genèrica, on es complia <nom>.cpp i resulta <nom>.o
	g++ -std=c++11 -c -o $@ $<
