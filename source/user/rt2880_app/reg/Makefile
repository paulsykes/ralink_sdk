EXEC = reg
OBJS = reg.o
CFLAGS += -I$(ROOTDIR)/$(LINUXDIR)/drivers/net/rt_rdm -I$(ROOTDIR)/$(LINUXDIR)/include

all: $(EXEC)

$(EXEC): $(OBJS)
	$(CC) $(LDFLAGS) -o $@ $(OBJS)

romfs:
	$(ROMFSINST) /bin/$(EXEC)

clean:
	-rm -f $(EXEC) *.elf *.gdb *.o

