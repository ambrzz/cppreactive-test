# Distributed under the OSI-approved BSD 3-Clause License.  See accompanying
# file Copyright.txt or https://cmake.org/licensing for details.

cmake_minimum_required(VERSION 3.12.3)

# We name the project and the target for the ExternalProject_Add() call
# to something that will highlight to the user what we are working on if
# something goes wrong and an error message is produced.

project(rxcpp-populate NONE)

include(ExternalProject)
ExternalProject_Add(rxcpp-populate
                     "UPDATE_DISCONNECTED" "False" "GIT_REPOSITORY" "https://github.com/ReactiveX/RxCpp"
                    SOURCE_DIR          "/home/david-montoro/CLionProjects/cppreactive/cmake-build-debug/_deps/rxcpp-src"
                    BINARY_DIR          "/home/david-montoro/CLionProjects/cppreactive/cmake-build-debug/_deps/rxcpp-build"
                    CONFIGURE_COMMAND   ""
                    BUILD_COMMAND       ""
                    INSTALL_COMMAND     ""
                    TEST_COMMAND        ""
)
