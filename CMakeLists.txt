cmake_minimum_required(VERSION 2.6.0)

# pull in the pods macros. See cmake/pods.cmake for documentation
set(POD_NAME gperftools-2.1)
include(cmake/pods.cmake)

pods_install_pkg_config_file( gperftools-2.1
    CFLAGS
    LIBS -ltcmalloc_minimal
    REQUIRES
    VERSION 0.0.1)
