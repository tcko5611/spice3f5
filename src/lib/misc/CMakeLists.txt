add_definitions(-DHAS_NO_IEEE_LOGB)
add_library(misc alloc.c     dup2.c   math.c    printnum.c  tilde.c
dos_dirs.c  ivars.c  mktemp.c  string.c    time.c)
