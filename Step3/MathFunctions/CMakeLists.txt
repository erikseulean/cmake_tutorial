add_library(MathFunctions mysqrt.cxx)

# TODO 1: State that anybody linking to MathFunctions needs to include the
# current source directory, while MathFunctions itself doesn't.
# Hint: Use target_include_directories with the INTERFACE keyword

# this specifies where and what are the headers needed when using this library
# that way you don't have to specify the includes manually in the libraries
# using this library
target_include_directories(MathFunctions INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})