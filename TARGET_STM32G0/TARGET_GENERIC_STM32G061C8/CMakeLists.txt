# Copyright (c) 2021 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-generic-stm32g061c8 INTERFACE)

target_sources(mbed-generic-stm32g061c8
    INTERFACE
        PeripheralPins.c
        system_clock.c
)

target_include_directories(mbed-generic-stm32g061c8
    INTERFACE
        .
)

target_link_libraries(mbed-generic-stm32g061c8 INTERFACE mbed-stm32g061x8)
