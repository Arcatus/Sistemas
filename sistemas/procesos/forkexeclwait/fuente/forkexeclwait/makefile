# % W %

COMPILADOR=gcc
FUENTE=forkexeclwait.c $(RUTA_UTIL)error.c
OBJS=$(FUENTE:.c=.o)
HEADER=forkexeclwait.h error.h
PROG=$(RUTA_BIN)forkexeclwait

$(PROG):$(OBJS)
	$(COMPILADOR) $(OBJS) -lm -o $@
	@-echo "Compilación terminada"
clean:
	@- rm -f $(OBJS)
	@- echo "Borrado de objetos terminado"
fclean:
	@- rm -f $(OBJS) $(PROG)
	@- echo "Borrado de archivos terminado"
.c.o:
	$(COMPILADOR) -c -I$(RUTA_INCL) $*.c -o $*.o
