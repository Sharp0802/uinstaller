
N := uins.out
C := $(wildcard *.c)
O := $(C:.c=.o)

$(N): $(O)
	$(LD) $(LDFLAGS) $^ -o $@

%.o: %.c
	$(CC) $(CFLAGS) $^ -o $@

clean:
	rm -rf $(O) $(N)

