# Copyright (C) 2015-2021, Wazuh Inc.
#
# This program is free software; you can redistribute it
# and/or modify it under the terms of the GNU General Public
# License (version 2) as published by the FSF - Free Software
# Foundation.

cmake_minimum_required(VERSION 3.10)

if(${TARGET} STREQUAL "server")
    add_subdirectory(shared)
    add_subdirectory(sha1)
    add_subdirectory(blowfish)
    add_subdirectory(md5)
    add_subdirectory(md5_sha1)
endif()
