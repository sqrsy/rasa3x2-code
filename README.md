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
* Positive output, with switches (PO-4S)
* Positive output, without switches (PO-0S)
* Thru-zero output, with switches (TZO-4S)
* Thru-zero output, without switches (TZO-0S)

Thru-zero output is kept optional because it requires more parts.

# PO-4S Programs

COMING EVENTUALLY!!

# PO-0S Programs

COMING EVENTUALLY!!

# TZO-4S Programs

COMING EVENTUALLY!!

# TZO-0S Programs

COMING EVENTUALLY!!

# Disclaimer

All files are provided without any guarantee. If you notice a mistake, please submit an Issue and I will fix it.