include_directories(${PROJECT_SOURCE_DIR}/src/include
  ${PROJECT_SOURCE_DIR}/src/lib/dev)

set(confc "${CMAKE_CURRENT_BINARY_DIR}/conf.c")
set(devices "asrc bjt bsim1 bsim2 cap cccs ccvs csw dio ind isrc jfet ltra mes mos1 mos2 mos3 mos6 res sw tra urc vccs vcvs vsrc")
set(analyses "op dc tf ac tran pz disto noise sense")
set(version "3f5")
add_executable(spice3 main.c ${confc} tune.c)
target_link_libraries (spice3 fte dev ckt cp hlp inp mfb ni misc sparse)
link_directories(${CMAKE_BINARY_DIR}/lib)
add_custom_command(
  OUTPUT ${confc}
  COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/mkvers.sh "${devices}" "${analyses}" "${version}" > ${confc}
  COMMAND cat ${CMAKE_CURRENT_SOURCE_DIR}/config.c >> ${confc}
  )

set(nconfc "${CMAKE_CURRENT_BINARY_DIR}/nconf.c")
add_executable(nutmeg main.c ${nconfc} tune.c)
target_link_libraries (nutmeg fte cp hlp mfb misc)
add_custom_command(
  OUTPUT ${nconfc}
  COMMAND ${CMAKE_CURRENT_SOURCE_DIR}/mkvers.sh "" "" "${version}" "" > ${nconfc}
  COMMAND cat ${CMAKE_CURRENT_SOURCE_DIR}/nconfig.c >> ${nconfc}
  )
