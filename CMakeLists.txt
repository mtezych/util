
cmake_minimum_required (VERSION 3.11)

project (Util VERSION 1.0.0 LANGUAGES CXX)


add_library                (util STATIC)

target_include_directories (util PUBLIC include)

target_compile_features    (util PUBLIC cxx_std_17)

target_sources             (util PRIVATE include/util/Util.h
                                               source/Util.cxx)
