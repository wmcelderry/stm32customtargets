# Copyright (c) 2021 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-generic-stm32h750zb INTERFACE)

target_sources(mbed-generic-stm32h750zb
    INTERFACE
        PeripheralPins.c
        system_clock.c
)

target_include_directories(mbed-generic-stm32h750zb
    INTERFACE
        .
)

target_link_libraries(mbed-generic-stm32h750zb INTERFACE mbed-stm32h750xb)
