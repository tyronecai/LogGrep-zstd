cc = g++
EXEC = THULR
SRCS = main.cpp sampler.cpp Coffer.cpp Encoder.cpp util.cpp LengthParser.cpp template.cpp union.cpp SubPattern.cpp timer.cpp
OBJS = $(SRCS:.cpp=.o)

LIBS = -lzstd

start:$(OBJS)
	$(cc) $(OBJS) -o $(EXEC) $(LIBPATH) $(LIBS) 
	rm -rf $(OBJS)
.cpp.o:
	$(cc) -I$(LIBDIR) -O2 -std=c++11 -g -Wall -o $@ -c $^ 
clean:
	rm -rf $(OBJS) $(EXEC)
