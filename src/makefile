all: prog clean
processos.o: processos.cpp defines.h
	g++ -c -Wall processos.cpp

memoria.o: memoria.cpp defines.h
	g++ -c -Wall memoria.cpp	

recursos.o: recursos.cpp defines.h
	g++ -c -Wall recursos.cpp

debug.o: debug.cpp defines.h
	g++ -c -Wall debug.cpp

utils.o: utils.cpp defines.h
	g++ -c -Wall utils.cpp

output.o: output.cpp defines.h
	g++ -c -Wall output.cpp

main.o: main.cpp defines.h
	g++ -c -Wall main.cpp



prog: utils.o main.o debug.o processos.o recursos.o memoria.o output.o
	g++ -g -Wall main.o utils.o debug.o processos.o recursos.o memoria.o output.o -o simulacao

clean:
	rm -f *.o
