add_library(mos3 mos3.c      mos3del.c   mos3ic.c    mos3mpar.c  mos3sacl.c  mos3sset.c
mos3acld.c  mos3dest.c  mos3load.c  mos3noi.c   mos3set.c   mos3supd.c
mos3ask.c   mos3dist.c  mos3mask.c  mos3par.c   mos3sld.c   mos3temp.c
mos3conv.c  mos3dset.c  mos3mdel.c  mos3pzld.c  mos3sprt.c  mos3trun.c)

include_directories(${PROJECT_SOURCE_DIR}/src/include)
target_link_libraries(mos3 dev ni)
