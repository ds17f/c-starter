CC=gcc
CFLAGS=-Wall -Wextra -std=c11
TARGET={{cookiecutter.project_name}}
DEBUG_FLAGS=-g -O0

all: $(TARGET)

$(TARGET): main.o
	$(CC) $(CFLAGS) -o $(TARGET) main.o

debug: CFLAGS += $(DEBUG_FLAGS)
debug: $(TARGET)

clean:
	rm -f $(TARGET) *.o

run: $(TARGET)
	./$(TARGET)
