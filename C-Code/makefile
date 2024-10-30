# Compiler und Flags
CC = gcc
CFLAGS = -Wall

# Dateien und Ausgabedatei
TARGET = mnist_inference
SRCS = main.c
HEADERS = trained_votes_long.h pixel_data.h
OBJS = $(SRCS:.c=.o)

# Regeln
all: $(TARGET)

$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJS)

%.o: %.c $(HEADERS)
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJS) $(TARGET)

predict: $(TARGET)
	./$(TARGET)

.PHONY: all clean predict
