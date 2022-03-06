# Libgpiod-GPIO
Creation of a book for this library has been postponed until the library has increased
functions, such as PWM and other commands. An alternative is to use the lgpio library 
at: https://github.com/eugenedakin/lgpio-GPIO

Raspberry Pi Libgpio for the Raspberry Pi 4 B with Xojo API 2

Created 26 Feb 2022: sysfs functions on the Raspberry Pi are being deprecated and the newer
Libgpio interface is the default standard. 

This is a Libgpio library that is a replacement for the deprecated wiringPi library that
is to be used with Xojo apps. Libgpiod is also a replacement for pigpoid since there are 
some legacy sysfs commands with interrupts with pigpiod. A book has been written called 
'I Wish I Knew How To...Program Raspberry Pi 4B Electronics with Xojo: Libgpiod and API2 Edition' is being written and the 
examples use this library exclusively. More instructions about the book will be available
at https://www.scispec.ca and press the button on books.

A historic review is that the first Raspberry Pi Electronics book for Xojo was written
with wiringPi in June of 2016. Many examples were added and updated from Raspberry Pi 2B and
Raspberry Pi 3B boards. Major updates to the book occured when Raspberry Pi 4B arrived with
the new operating system. As of June 2020 the Operating System was Raspberry Pi OS, with Raspberry Pi 4B, 
using Xojo's 2019 R3.1 (Xojo API2) code. 

With the changes in Raspberry Pi motherboard, Raspberry Pi Opeating System, Xojo API2, 
deprecation of sysfs, and deprecation of wiringPi, a new book is being written that 
provides examples, explanations, and data for all of these recent changes. 

The book is currently being written as of Feb 2022. 

V 1.0 26 Feb 2022 Edition (5.0)
The initial and starting declares used to work with the GPIO on Raspberry Pi 4, 
with Xojo 2021 r3.1, with the Raspberry Pi Operating System, and uses the
Libgpio library that is sepearately installed onto the Raspberry Pi operating system. 
As the writing of the book progresses, so will the versions of this method. 

V1.0 (26 Feb 2022)
 - Wrote gpiod_chip_open
 - Wrote gpoid_chip_open_by_name
 - Wrote gpiod_line_request_output
 - Wrote gpoid_chip_get_line
 - Wrote gpiod_chip_close
 - Wrote gpiod_line_release
 - Wrote gpiod_line_set_value
 - Added Input constant
 - Added Output constant
 - Added On constant
 - Added Off constant

Updated
v1.1 (27 Feb 2022)
 - Added GPIOD_CTXLESS_FLAG_OPEN_DRAIN
 - Added GPIOD_CTXLESS_FLAG_OPEN_SOURCE
 - Added GPIOD_CTXLESS_FLAG_BIAS_PULL_UP
 - Added GPIOD_CTXLESS_FLAG_BIAS_PULL_DOWN
 - Added GPIOD_CTXLESS_FLAG_BIAS_DISABLE
 - Added GPIOD_LINE_ACTIVE_STATE_HIGH
 - Added GPIOD_LINE_ACTIVE_STATE_LOW
 - Added GPIOD_CTXLESS_EVENT_CB_TIMEOUT
 - Added GPIOD_CTXLESS_EVENT_CB_RISING_EDGE
 - Added GPIOD_CTXLESS_EVENT_CB_FALLING_EDGE
 - Added GPIOD_CTXLESS_EVENT_POLL_RET_STOP
 - Added GPIOD_CTXLESS_EVENT_POLL_RET_ERR
 - Added GPIOD_CTXLESS_EVENT_POLL_RET_TIMEOUT
 - Added GPIOD_LINE_BIAS_AS_IS
 - Added GPIOD_LINE_BIAS_DISABLE
 - Added GPIOD_LINE_BIAS_PULL_UP
 - Added GPIOD_LINE_BIAS_PULL_DOWN
 - Added GPIOD_LINE_DIRECTION_INPUT
 - Added GPIOD_LINE_DIRECTION_OUTPUT
 - Added GPIOD_LINE_EVENT_RISING_EDGE
 - Added GPIOD_LINE_EVENT_FALLING_EDGE
 - Added GPIOD_LINE_REQUEST_FLAG_OPEN_DRAIN
 - Added GPIOD_LINE_REQUEST_FLAG_OPEN_SOURCE
 - Added GPIOD_LINE_REQUEST_FLAG_ACTIVE_LOW
 - Added GPIOD_LINE_REQUEST_FLAG_BIAS_DISABLE
 - Added GPIOD_LINE_REQUEST_FLAG_BIAS_PULL_DOWN
 - Added GPIOD_LINE_REQUEST_FLAG_BIAS_PULL_UP
 - Added GPIOD_BIT Function 
 - Added gpiod_line_request_input
 - Added gpiod_line_get_value

Updated v1.2 (4 Mar 2022)

 - Added comments to gpiod_line_request_output
 - Added gpiod_line_request_output_flags
 - Changed gpiod_line_request_output third parameter for On and Off
 - Added gpiod_line_request_input_flags
 - Added gpiod_line_set_flags
