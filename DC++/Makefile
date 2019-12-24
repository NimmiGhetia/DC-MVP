CC = gcc

OFILES = client.o \
	server.o 

CFILECLT = client.c

CFILESRV = server.c

EXESRV = server

EXECLT = client

but : ${EXESRV} ${EXECLT}

${EXESRV} :
	$(CC) $(CFLAGS) -o ${EXESRV} ${CFILESRV} -lpthread

${EXECLT} :
	$(CC) $(CFLAGS) -o ${EXECLT} ${CFILECLT}

clean :
	-rm -f ${OFILES} ${EXESRV} ${EXECLT} *~
                 
rmproper : clean but

.PHONY : but clean rmproper
