.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = helloecho
DEBUG_EXEC    = helloecho-dbg
SOURCE        = helloecho.cpp

all: debug release

debug: $(DEBUG_EXEC)

$(DEBUG_EXEC): helloecho.cpp
	g++ $(DEBUG_FLAGS) helloecho.cpp -o $(DEBUG_EXEC) 

release: $(RELEASE_EXEC)

$(RELEASE_EXEC): helloecho.cpp
	g++ $(RELEASE_FLAGS) helloecho.cpp -o $(RELEASE_EXEC)

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC)
