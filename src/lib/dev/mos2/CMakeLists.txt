add_library(mos2 mos2.c      mos2del.c   mos2ic.c    mos2mpar.c  mos2sacl.c  mos2sset.c
mos2acld.c  mos2dest.c  mos2load.c  mos2noi.c   mos2set.c   mos2supd.c
mos2ask.c   mos2dist.c  mos2mask.c  mos2par.c   mos2sld.c   mos2temp.c
mos2conv.c  mos2dset.c  mos2mdel.c  mos2pzld.c  mos2sprt.c  mos2trun.c)
target_link_libraries(mos2 disto)
