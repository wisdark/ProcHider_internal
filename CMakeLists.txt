cmake_minimum_required(VERSION 3.19)
project(ProcHider_internal C)

set(CMAKE_C_STANDARD 99)
#Disable warnings that occur due to phnt
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wno-pragma-pack -Wno-microsoft-enum-forward-reference -Wno-visibility")
add_library(ProcHider_internal SHARED src/dllmain.c src/hook.h src/hook.c)

include_directories("C:/NextCloud/Code/includes/phnt")
