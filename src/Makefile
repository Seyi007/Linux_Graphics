# Compiler
CXX = g++
CXXFLAGS = -I/home/seyik/learnopengl/include
LDFLAGS = -ldl -lglfw -lGL

# Source files
SRC = $(wildcard *.cpp)
OUT = $(SRC:.cpp=)

# Default target: build all executables
all: $(OUT)

# Rule to build each executable
%: %.cpp glad.c
	$(CXX) $^ $(CXXFLAGS) $(LDFLAGS) -o $@

# Clean build files
clean:
	rm -f $(OUT) *.o
