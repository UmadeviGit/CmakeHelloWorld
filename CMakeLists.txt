cmake_minimum_required(VERSION "3.23.0-rc1")

project("HelloWorld")

add_executable("${PROJECT_NAME}" "HelloWorld.cpp")
set(CPACK_GENERATOR WIX)
set(CPACK_PACKAGE_NAME "mydll")
set(CPACK_PACKAGE_VENDOR "CMake.org")
set(CPACK_PACKAGE_DESCRIPTION_SUMMARY "MyLib - CPack Component Installation Example")
set(CPACK_PACKAGE_VERSION "1.0.0")
set(CPACK_PACKAGE_VERSION_MAJOR "1")
set(CPACK_PACKAGE_VERSION_MINOR "0")
set(CPACK_PACKAGE_VERSION_PATCH "0")
set(CPACK_PACKAGE_INSTALL_DIRECTORY "CPack Component Example")

INCLUDE(CPack)
