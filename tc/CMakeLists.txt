include_directories(.)

add_subdirectory(lang)
add_subdirectory(proto)
add_subdirectory(version)
add_subdirectory(core)
add_subdirectory(autotuner)
add_subdirectory(aten)

if (WITH_CAFFE2 AND WITH_CUDA)
  add_subdirectory(c2)
endif()
