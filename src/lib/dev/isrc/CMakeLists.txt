add_library(isrc isrc.c      isrcacld.c  isrcdel.c   isrcload.c  isrcpar.c
isrcacct.c  isrcask.c   isrcdest.c  isrcmdel.c  isrctemp.c)

include_directories(${PROJECT_SOURCE_DIR}/src/include)
target_link_libraries(isrc ckt)
