# Copyright (c) 2021 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-generic-stm32h7a3qiq INTERFACE)

target_sources(mbed-generic-stm32h7a3qiq
    INTERFACE
        PeripheralPins.c
        system_clock.c
)

target_include_directories(mbed-generic-stm32h7a3qiq
    INTERFACE
        .
)

target_link_libraries(mbed-generic-stm32h7a3qiq INTERFACE mbed-stm32h7a3xiq)
