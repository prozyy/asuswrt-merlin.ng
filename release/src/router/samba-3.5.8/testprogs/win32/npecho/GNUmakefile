INCLUDES=-I.
CFLAGS=$(INCLUDES)

NPECHO = npecho_client.exe
#npecho_server.exe

NPECHO2 = npecho_client2.exe npecho_server2.exe

all: $(NPECHO) $(NPECHO2)

CC = i586-mingw32msvc-gcc

.SUFFIXES: .c .obj .exe

.c.obj:
	$(CC) $(CFLAGS) -c $< -o $@

.obj.exe:
	$(CC) $(CFLAGS) -o $@ $< $(LIBS)

clean:
	del *~ *.obj *.exe

