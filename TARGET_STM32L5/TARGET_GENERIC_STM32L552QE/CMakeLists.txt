# Copyright (c) 2021 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-generic-stm32l552qe INTERFACE)

target_sources(mbed-generic-stm32l552qe
    INTERFACE
        PeripheralPins.c
        system_clock.c
)

target_include_directories(mbed-generic-stm32l552qe
    INTERFACE
        .
)

target_link_libraries(mbed-generic-stm32l552qe INTERFACE mbed-stm32l552xe)
