# SPDX-FileCopyrightText: (C) 2022 Cem Geçgel <gecgelcem@outlook.com>
# SPDX-License-Identifier: GPL-3.0-or-later

cmake_minimum_required(VERSION 3.21.2)

project(glad)
add_library(${PROJECT_NAME} STATIC
src/gl.c
include/glad/gl.h
include/KHR/khrplatform.h
)
target_include_directories(${PROJECT_NAME} PUBLIC include)
