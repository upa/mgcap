TARGET = mgdump

CFLAGS = -Wall -O2

SRCS := mgdump.c
OBJS = $(subst .c,.o,$(SRCS))

${TARGET}: ${OBJS}
	$(CC) ${LDFLAGS} -o $@ $^

.c.o:
	$(CC) ${CFLAGS} -o $@ -c $<

.PHONY: clean
clean:
	rm -f ${TARGET} ${OBJS}

