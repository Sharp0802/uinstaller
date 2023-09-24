
CC := cc
LD := ld

N := uins.out
C := $(wildcard *.c)
O := $(C:.c=.o)

all: $(N)

$(N): $(O)
	$(LD) $(LDFLAGS) -lc $^ -o $@

%.o: %.c
	$(CC) $(CFLAGS) -c $^ -o $@

clean:
	rm -rf $(O) $(N)

.PHONY: all clean
