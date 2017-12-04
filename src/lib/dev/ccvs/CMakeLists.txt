add_library(ccvs ccvs.c     ccvsdest.c  ccvsmdel.c  ccvssacl.c  ccvssprt.c
ccvsask.c  ccvsfbr.c   ccvspar.c   ccvsset.c   ccvssset.c
ccvsdel.c  ccvsload.c  ccvspzld.c  ccvssld.c)
include_directories(${PROJECT_SOURCE_DIR}/src/include)
target_link_libraries(ccvs ckt)
