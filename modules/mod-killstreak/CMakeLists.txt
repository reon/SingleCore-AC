CU_SET_PATH("CMAKE_MOD_KILLSTREAK_DIR" "${CMAKE_CURRENT_LIST_DIR}")

AC_ADD_SCRIPT("${CMAKE_CURRENT_LIST_DIR}/src/mod_killstreak.cpp")

AC_ADD_SCRIPT_LOADER("KillstreakSystem" "${CMAKE_CURRENT_LIST_DIR}/src/loader_killstreak.h")

CU_ADD_HOOK(AFTER_WORLDSERVER_CMAKE "${CMAKE_CURRENT_LIST_DIR}/src/cmake/after_ws_install.cmake")