include ../config.mk

SRC = text.c ../text.c
SRC += $(wildcard ccan/*/*.c)
INCS += -I..

test: text
	@./text

text: *.c
	@echo ${CC} ${CFLAGS} ${SRC} ${LDFLAGS} -o $@
	@${CC} ${CFLAGS} ${SRC} ${LDFLAGS} -o $@

debug: clean
	@$(MAKE) CFLAGS='${DEBUG_CFLAGS}'

clean:
	@echo cleaning
	@rm -f text

.PHONY: clean debug
