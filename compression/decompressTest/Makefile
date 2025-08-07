cc = g++
EXEC = DeCompressor
SRCS = main.cpp ../Coffer.cpp
OBJS = $(SRCS:.cpp=.o)

LIBS = -lzstd

start:$(OBJS)
	  $(cc) $(OBJS) $(LIB) -o $(EXEC) $(LIBS)
.cpp.o:
	$(cc) -O0 -c -I$(LIBDIR) -std=c++11 -g -Wall -o $@ -c $^ 
clean:
	rm -rf $(OBJS) $(EXEC)
