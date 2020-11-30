cmake_minimum_required(VERSION 3.16)
project(wiringPi C)

set(CMAKE_C_STANDARD 11)

add_link_options(-lm -lpthread -lrt -lcrypt)

add_library(wiringPi SHARED
        wiringPi/wiringPi.c
        wiringPi/wiringPi.h
        wiringPi/wiringSerial.c
        wiringPi/wiringShift.c
        wiringPi/piHiPri.c
        wiringPi/piThread.c
        wiringPi/wiringPiSPI.c
        wiringPi/wiringPiI2C.c
        wiringPi/softPwm.c
        wiringPi/softTone.c
        wiringPi/mcp23008.c
        wiringPi/mcp23016.c
        wiringPi/mcp23017.c
        wiringPi/mcp23s08.c
        wiringPi/mcp23s17.c
        wiringPi/sr595.c
        wiringPi/pcf8574.c
        wiringPi/pcf8591.c
        wiringPi/mcp3002.c
        wiringPi/mcp3004.c
        wiringPi/mcp4802.c
        wiringPi/mcp3422.c
        wiringPi/max31855.c
        wiringPi/max5322.c
        wiringPi/ads1115.c
        wiringPi/sn3218.c
        wiringPi/bmp180.c
        wiringPi/htu21d.c
        wiringPi/ds18b20.c
        wiringPi/rht03.c
        wiringPi/drcSerial.c
        wiringPi/drcNet.c
        wiringPi/pseudoPins.c
        wiringPi/wpiExtensions.c
        )
