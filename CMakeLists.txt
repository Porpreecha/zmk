cmake_minimum_required(VERSION 3.13.1)
find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(my_6x15)

target_sources(app PRIVATE
    config/my_6x15.keymap
    boards/arm/nice_nano_v2.dts
)
