# What is it?

The 'Rasa3x2' is a 10HP Eurorack module built around the Arduino Nano Every. The circuit is very simple, but can be used to perform a number of tasks helpful in music synthesis. My intent was to design a standard module that could be easily programmed by anyone in the DIY music scene, even those with limited software or hardware skills. All code is open source, freely available for you to use and modify. If you make a cool module using the 'Rasa3x2' module -- or some cool music -- let me know and I will link it here.

# About the 'Rasa3x2'

The 'Rasa3x2' circuit is very simple. It has 4 jacks, 4 switches, and 6 pots.
* Jacks 1 & 2: For reading input. Voltage divider steps 0-12V down to 0-5V so your Arduino doesn't get fried.
* Pots 1-6: For setting parameters. Reads 0-5V that can be mapped to module parameters.
* Switches 1-4: For setting parameters. The switches are optional.
* Jacks 3 & 4: For sending output. The module uses an MCP4822 Digital-to-Analog converter (DAC). You can install an optional op-amp sub-module to output thru-zero voltage.

# Configurations

The 'Rasa3x2' can be configured in 4 modes:
(1) Positive output, with switches
(2) Positive output, without switches
(3) Thru-zero output, with switches
(4) Thru-zero output, without switches

Activating thru-zero output requires more parts. It is optional, and not necessary for programs like envelope generators.

# Programs for "Positive output, with switches"

COMING EVENTUALLY!!

# Programs for "Positive output, without switches"

COMING EVENTUALLY!!

# Programs for "Thru-zero output, with switches"

COMING EVENTUALLY!!

# Programs for "Thru-zero output, without switches"

COMING EVENTUALLY!!

# Disclaimer

All files are provided without any guarantee. If you notice a mistake, please submit an Issue and I will fix it.