
file(GLOB lua_source_files "*.c")

list(FILTER lua_source_files EXCLUDE REGEX "lua.c")

add_library(Lua STATIC ${lua_source_files})