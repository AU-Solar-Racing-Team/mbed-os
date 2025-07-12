# Copyright (c) 2020 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(mbed-vcmv1 INTERFACE)

target_sources(mbed-vcmv1
    INTERFACE
        PeripheralPins.c
)

target_include_directories(mbed-vcmv1
    INTERFACE
        .
)

target_link_libraries(mbed-vcmv1 INTERFACE mbed-stm32u575xg)
