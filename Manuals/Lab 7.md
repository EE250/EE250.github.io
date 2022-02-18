# Lab 07: ADC and DAC 
### Mixed-Signal Circuit Simulation

Files to submit via Vocareum: 
- `adc_circuit_schematic.png`
- `dac_circuit_schematic.png`
- `Lab07_writeup.txt`
- include a link to a video (with narration) of your lab demo. Please check the rubric for what your video must demonstrate.

Students in teams must submit on Vocareum as a team:

### Introduction
This lab gets you to create schematics for and simulate two circuits that we have discussed in class. The first circuit will be an analog to digital converter (ADC) that will take an analog voltage signal and output the corresponding digital output in bits. The second circuit is a digital to analog converter (DAC) that will do the reverse operation - take a set of bits and produce an analog voltage corresponding to the input. 

### Setup
For this lab you will need to first get yourself a free account on https://www.multisim.com/

Once you create an account, log in and select “Create Circuit”. You can now drag and drop the parts from the menu on the left on to the schematic editor, and wire them up using the wiring tool.  Go through the [getting started tutorial](https://www.multisim.com/get-started/) on the multisim site to become familiar with the editor.

### Part 1: Analog to Digital Converter (ADC)

Your first task is to create and simulate a parallel comparator type ADC, also known as a Flash-type ADC. Read and recreate the circuit described in [this tutorial](https://www.electronics-tutorial.net/analog-integrated-circuits/data-converters/flash-type-adc/) which converts an input voltage to 2 bits.

Use a DC voltage source providing 20 volts for the circuit (V). And use another DC voltage source to the analog input voltage (Vin). For the digital logic gates, have the high voltage correspond to 5 volts, and low to 0 volts.  Connect voltage probes to the output of the logic gates. 

**Question 1**:  *Explain what the set of four resistors are there for.* 

First verify that  with the circuit, analog input voltage values from 0 to 5 volt give a 2-bit output of “00”, values from 5 to 10 volt yield “01”, values from 10 to 15 volt yield “10” and values from 15 to 20 volt result in an output of “11”. 

Export the schematic to a png file, name it adc_circuit_schematic.png  this will be part of your submission. 

**Question 2**:  Say for some reason a non-uniform ADC is desired, such that 
- analog input values from 0 to 12 volts result in “00”
- values from 12 to 15 volts result in “01”
- values from 15 to 18 volts result in “10” 
- values from 18 to 20 volts result in “11”

*What should the values of the 4 resistors be in order to make this happen?*

**Question 3**: *How many resistors are needed if you wanted to extend this design to make an 8-bit ADC?*

### Part 2: Digital to Analog Converter (DAC)

Your second task is to create and simulate a 3-bit binary weighted resistor DAC. Read and recreate the circuit described [here](https://www.electronics-tutorial.net/analog-integrated-circuits/data-converters/binary-weighted-resistor-dac/).

Let the 3-bit input digital voltages be each represented by 5 volts for 1 and 0 volts for a “0”. 
Use a single pole double throw (SPDT) switch to set each input bit to either “0” or “1”. 

At the output of the circuit, add an inverting op-amp with [appropriate choice of resistors](https://www.electronics-tutorial.net/amplifier/inverting-amplifier/) so that the final output voltage is between 0 to 20 volts. 

Export the schematic to a png file, name it `dac_circuit_schematic.png`. This will be part of your submission. 

**Question 4**: *If you were to extend the circuit design to an 8-bit DAC, how many resistors would it require?*   

**Question 5**: Say you were to extend the circuit design to an 8-bit DAC and the smallest resistor in the weighted binary resistor bank had the value of 1kohm. *What would be the value of the largest resistor in the weighted binary resistor bank?*

### Rubrics
All files are to be submitted via Vocareum in teams. 
For recording your demo video we recommend using Zoom.

| Points         | Description | 
| -------------- | ----------- |
| **Schematics** |             |
| 1              | Circuit schematic for ADC looks clean and professional |
| 1              | Circuit schematic for DAC looks clean and professional |
| **Demo Video** |             |
| 4              | For the ADC circuit, with all resistors set to the same value, show the 2-bit output is correct using a voltage probe for four different values of the input corresponding to each possible output value. |
| 4              | Show using a voltage probe that the output is correct for all 8 possible values of the 3-bit input in the DAC circuit. |
| **Questions**  |             |
| 2              | Question 1 |
| 2              | Question 2 |
| 2              | Question 3 |
| 2              | Question 4 |
| 2              | Question 5 |

Total Possible: 20