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

The following programs are currently available:

* Dual Envelope:
	* Author: sqrsy
	* Purpose: Generates an ADSR envelope from a gate signal.
	* Jack 1 (top left): Clock in. Triggers Envelope 1.
	* Pot 1 (top left): Controls attack rate for Envelope 1.
	* Pot 2 (middle left): Controls decay and release rate for Envelope 1.
	* Pot 3 (bottom left): Controls sustain level for Envelope 1.
	* Switch 1: Increases attack length for Envelope 1.
	* Switch 2: Increases decay and release length for Envelope 1.
	* Jack 2 (top right): Clock in. Triggers Envelope 2.
	* Pot 4 (top right): Controls attack rate for Envelope 2.
	* Pot 5 (middle right): Controls decay and release rate for Envelope 2.
	* Pot 6 (bottom right): Controls sustain level for Envelope 2.
	* Switch 3: Increases attack length for Envelope 2.
	* Switch 4: Increases decay and release length for Envelope 2.
	* Jack 3: Envelope 1 out.
	* Jack 4: Envelope 2 out.

# PO-0S Programs

The following programs are currently available:

* Dual Envelope:
	* Author: sqrsy
	* Purpose: Generates an envelope based on samples from a children's toy.
	* Jack 1 (top left): Clock in. Triggers Envelope 1.
	* Pot 1 (top left): Sets Envelope 1 to any of 20 envelopes in the sample bank.
	* Pot 2 (middle left): Controls the speed of sample playback for Envelope 1.
	* Pot 3 (bottom left): Controls the delay before starting Envelope 1.
	* Jack 2 (top right): Clock in. Triggers Envelope 2.
	* Pot 4 (top right): Sets Envelope 2 to any of 20 envelopes in the sample bank.
	* Pot 5 (middle right): Controls the speed of sample playback for Envelope 2.
	* Pot 6 (bottom right): Controls the delay before starting Envelope 2.
	* Jack 3: Envelope 1 out.
	* Jack 4: Envelope 2 out.

# TZO-4S Programs

COMING EVENTUALLY!!

# TZO-0S Programs

* Modulated LFO:
	* Author: sqrsy
	* Purpose: Generates a LFO that is modulated by an Envelope.
	* Jack 1 (top left): Clock in. Triggers Envelope.
	* Pot 1 (top left): Controls attack rate for Envelope.
	* Pot 2 (middle left): Controls decay and release rate for Envelope.
	* Pot 3 (bottom left): Controls sustain level for Envelope.
	* Jack 2 (top right): CV in. Increases frequency of LFO (up to 3x speed).
		* Note: CV will increase frequency on top of Envelope FM up to max speed.
	* Pot 4 (top right): Interpolates between triangle LFO and noise LFO.
	* Pot 5 (middle right): Controls the base speed of LFO.
	* Pot 6 (bottom right): Allows Envelope to increase frequency of LFO (up to 3x speed).
	* Jack 3: Envelope out.
	* Jack 4: LFO out.

# Disclaimer

All files are provided without any guarantee. If you notice a mistake, please submit an Issue and I will fix it.