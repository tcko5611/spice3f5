add_library(dev devsup.c)

target_link_libraries(dev  ccvs             isrc       mos3           urc
 asrc                jfet       mos6           vccs
 bjt                 csw            ltra          vcvs
 bsim1               res            vsrc
 bsim2               dio              mes        
 cap                 disto            mos1       sw
 cccs                ind              mos2       tra )
include_directories(${PROJECT_SOURCE_DIR}/src/include)
add_subdirectory(ccvs)
add_subdirectory(isrc)
add_subdirectory(mos3)
add_subdirectory(urc)
add_subdirectory(asrc)
add_subdirectory(jfet)
add_subdirectory(mos6)
add_subdirectory(vccs)
add_subdirectory(bjt)
add_subdirectory(csw)
add_subdirectory(ltra)
add_subdirectory(vcvs)
add_subdirectory(bsim1)
add_subdirectory(res)
add_subdirectory(vsrc)
add_subdirectory(bsim2)
add_subdirectory(dio)
add_subdirectory(mes)
add_subdirectory(cap)
add_subdirectory(disto)
add_subdirectory(mos1)
add_subdirectory(sw)
add_subdirectory(cccs)
add_subdirectory(ind)
add_subdirectory(mos2)
add_subdirectory(tra)


