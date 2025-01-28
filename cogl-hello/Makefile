
APP := cogl-hello

COGL_VER := cogl-2.0-experimental
CFLAGS := $(shell pkg-config --cflags $(COGL_VER) )
LDFLAGS := $(shell pkg-config --libs $(COGL_VER) )

all: $(APP)
$(APP): $(APP).c

clean:
	rm -f $(APP)

.PHONY: all clean
