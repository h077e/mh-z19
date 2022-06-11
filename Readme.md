# MH-Z19 Sensor with USB Connection on a x86 Linux PC

## Description

 The Program read the values as co2 concentration or temperature from MH-Z19 sensor.

 It's a version for my x86 Linux PC and a connected FT232RL usb-serial converter.

 The original source for Raspberry Pi found here: https://raw.githubusercontent.com/UedaTakeyuki/slider/master/mh_z19.py

## Examples

 * **execute without options**
	h077e@pc23:~/MH-19z$ sudo python -m mh_z19
	{"co2": 458}

 * **excecute with all functions**
	h077e@pc23:~/MH-19z$ sudo python -m mh_z19 --all
	{"SS": 0, "UhUl": 0, "TT": 63, "co2": 459, "temperature": 23}

 * **execute without structured output, only value**
	h077e@pc23:~/MH-19z$ sudo python -m mh_z19 --co2valueonly
	458
