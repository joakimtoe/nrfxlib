ble_controller
###############################

ble_controller is an RTOS-agnostic Bluetooth Low Energy controller
binary library, built for Nordic Semiconductor nRF52 Series SoCs.

The following library variants are available:

- libble_controller_s112_nrf52
	- Intended for nRF52810 and nRF52832.
	- Supports peripheral role only.
- libble_controller_s132_nrf52
	- Intended for nRF52810 and nRF52832.
	- Supports both peripheral and central roles.
	- Supports a maximum of one peripheral and two central links.
- libble_controller_s140_nrf52
	- Intended for nRF52840.
	- Supports both peripheral and central roles.
	- Supports a maximum of one peripheral and two central links.
	- Supports Coded PHY.

Each library is distributed in soft-float, softfp-float, and hard-float builds.

Integration notes
*****************
The controller library must be the only user of each the following peripherals:
	- RTC0
	- TIMER0
	- RADIO
	- POWER/CLOCK
	- SWI5
	- RNG

Disclaimer
**********
- The libraries are for evaluation purposes only.
- The libraries are not fully functional.
- The libraries are not built for performance.
