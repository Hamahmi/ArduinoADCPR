# ArduinoADCPR

- This is an Arduino Project written in AVR assembly code. The code takes an analog signal from
a Photoresistor and converts it to a digital signal that controls an LED.
- In simple words, if connected properly, the LED is ON when it is dark and it is off when there is
a light.
- Arduino Mega 2560 is used. Atmel Studio 7.0 is used to burn the code on the Arduino Mega
device.
- The code starts by initializing the ports by setting the corresponding DDR registers for each
port to set its mode (input or output). It configures internal registers to use pull-up resistors for
input pins. The code also sets up the analog-to-digital converter by initializing the ADC
variables.
- The code continuously waits for the ADC conversion to complete and then a threshold of 768 is
used to check brightness. Depending on the value, the LED is subsequently turned on or off.
- READ_ADC is responsible for reading the output of the ADC converter. KEEP_POLING is
used to continuously poll the value.
- ZERO turns the LED off, and ONE turns the led on.
- The physical hardware components we have used are the Photoresistor and the LED.
- A Photoresistor (or light-dependent resistor, LDR, or photo-conductive cell) is a light-controlled
variable resistor. The resistance of a Photoresistor decreases with increasing incident light
intensity; in other words, it exhibits photoconductivity. A Photoresistor can be applied in lightsensitive
detector circuits, and light-activated and dark-activated switching circuits.
- A light-emitting diode (LED) is a two-lead semiconductor light source. It is a p–n junction
diode that emits light when activated. When a suitable current is applied to the leads, electrons
are able to recombine with electron holes within the device, releasing energy in the form of
photons. This effect is called electroluminescence, and the color of the light (corresponding to
the energy of the photon) is determined by the energy band gap of the semiconductor. LEDs are
typically small (less than 1 mm2) and integrated optical components may be used to shape the
radiation pattern.
- We have also used resistors to prevent an overflow of voltage into the LED and the
Photoresistor, which could lead to burning the devices.
