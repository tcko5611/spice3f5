add_library(sparse spalloc.c  spextra.c   spoutput.c  spsolve.c
spbuild.c  spfactor.c  spsmp.c     sputils.c)
include_directories(${PROJECT_SOURCE_DIR}/src/include)
target_link_libraries(sparse misc)
