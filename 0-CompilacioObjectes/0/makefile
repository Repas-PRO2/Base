all: prog

clean: # netejem objectes (en aquest cas no n'hi ha)
	rm -rf *.o

ultraclean: clean # netejem objectes i programa
	rm -rf prog

#####

prog: main.cpp # compilem programa
	g++ -std=c++11 main.cpp -o prog
