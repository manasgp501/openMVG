
add_executable(openMVG_main_ColHarmonize main_ColHarmonize.cpp
  colorHarmonizeEngineGlobal.cpp)
target_link_libraries(openMVG_main_ColHarmonize
  lemon
  openMVG_features
  openMVG_image
  openMVG_kvld
  openMVG_lInftyComputerVision
  openMVG_sfm
  openMVG_system
  stlplus
  )

set_property(TARGET openMVG_main_ColHarmonize PROPERTY FOLDER OpenMVG/software)

install(TARGETS openMVG_main_ColHarmonize DESTINATION bin/)
