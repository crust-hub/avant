message("external start")
add_library(avant-http-parser SHARED "./http-parser/http_parser.c")

file(GLOB_RECURSE SOURCE_INIFILE "./avant-inifile/*.cpp")
add_library(avant-inifile SHARED ${SOURCE_INIFILE})


file(GLOB_RECURSE SOURCE_LOG "./avant-log/*.cpp")
add_library(avant-log SHARED ${SOURCE_LOG})

file(GLOB_RECURSE SOURCE_TIMER "./avant-timer/*.cpp")
add_library(avant-timer SHARED ${SOURCE_TIMER})

file(GLOB_RECURSE SOURCE_XML "./avant-xml/*.cpp")
add_library(avant-xml SHARED ${SOURCE_XML})

file(GLOB_RECURSE SOURCE_BUFFER "./avant-buffer/*.cpp")
add_library(avant-buffer SHARED ${SOURCE_BUFFER})

file(GLOB_RECURSE SOURCE_LUA "./lua/*.c")
add_library(avant-lua SHARED ${SOURCE_LUA})

file(GLOB_RECURSE SOURCE_ZLIB "./zlib/*.c")
add_library(avant-zlib SHARED ${SOURCE_ZLIB})

file(GLOB_RECURSE SOURCE_JSON "./avant-json/*.cpp")
add_library(avant-json SHARED ${SOURCE_JSON})

message("external end")
