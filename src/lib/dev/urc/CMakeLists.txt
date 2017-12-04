add_library(urc urc.c     urcdel.c   urcmask.c  urcmpar.c   urcsetup.c
urcask.c  urcdest.c  urcmdel.c  urcparam.c)
target_link_libraries(urc ckt)
