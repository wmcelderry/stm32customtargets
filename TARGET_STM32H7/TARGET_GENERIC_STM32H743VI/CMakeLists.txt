# Copyright (c) 2021 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-generic-stm32h743vi INTERFACE)

target_sources(mbed-generic-stm32h743vi
    INTERFACE
        PeripheralPins.c
        system_clock.c
)

target_include_directories(mbed-generic-stm32h743vi
    INTERFACE
        .
)

target_link_libraries(mbed-generic-stm32h743vi INTERFACE mbed-stm32h743xi)
