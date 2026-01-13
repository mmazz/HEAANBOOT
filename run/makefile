CXX = g++
CXXFLAGS = -std=c++11 -O2 -I../src
LDFLAGS = -L../lib -lntl -lgmp -lm

TARGET = HEAAN
SOURCES = run.cpp
LIB = ../lib/libHEAAN.a

$(TARGET): $(SOURCES)
	$(CXX) $(CXXFLAGS) $(SOURCES) $(LIB) $(LDFLAGS) -o $(TARGET)

clean:
	rm -f $(TARGET)
