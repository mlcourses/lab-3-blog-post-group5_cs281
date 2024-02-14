# Lab 03: Creating Sequential Patterns with Digital Circuit Design

## What We Did In The Last Lab

In the last lab - **Intro to Digital Design**, we delved into the intricacies of digital circuits, starting with the creation of a 2 to 1 mux using fundamental logic gates like AND, OR, and NOT gates. Progressing further, we utilized a 74150 mux chip to construct a more sophisticated 4 to 1 mux, ensuring meticulous wiring based on comprehensive diagrams and documentation. Integrating Arduino, we then employed it to control and test the mux's functionality, programming it to manage input data and control lines while validating output accuracy through systematic testing. Lastly, we designed and implemented a 1-bit adder circuit, demonstrating our proficiency in combining logic gates for arithmetic operations. For more in-depth lab details, refer to the previous lab in this [URL](https://github.com/mlcourses/lab-2-blog-post-group5_cs281/blob/main/post.md)

## Overview and Motivation

In this lab, we'll delve into constructing a circuit that displays numbers on a 7-segment LED based on a knob's position, much like a volume control. The lab starts with some groundwork, where we simplify circuit designs and understand how to represent numbers using a special kind of light display. The main part of the lab involves building a "ramp circuit," which means that as we turn the knob, the numbers displayed on the LED will gradually increase or decrease. We use a device called an Arduino to help with this, which turns the knob's movement into a digital signal. Then, we'll figure out how to use this digital signal to light up the correct LEDs on the 7-segment display. It's a mix of figuring out how to talk to the Arduino, designing the logic for the LED display, and putting it all together on a breadboard. The challenge is to make sure that as we turn the knob, the right numbers light up on the display.

<img src="./assets/overview.png" alt="overview" />

## Lab Objectives

1. Understand the function and operation of a 7-segment display for digital number representation.

2. Construct truth tables to indicate the outputs for each LED segment ion the 7-segment display. 

3. Use Karnaugh Maps to design and optimize the circuit's logics.

4. Use logisim to design and test a boolean circuit that combines the minimized functions for each LED segment.

5. Construct and test a voltage divider circuit using a potentiometer to generate analog input signals.

6. Implement combinational logic circuits to light up the 7-segment display.

7. Use Arduino to interpret digital signals and power the circuit. 

## Materials

- PB-503 breadboard prototyping station

- 7-segment display

- Arduino microcontroller

- 7404 NOT gate IC

- 7408 AND gate IC

- Two 7432 OR gate ICs

- IC data sheets

- Wires and connection tools

- Logic Probes

- Arduino IDE software

- USB cable

- Laptop or device for programming and powering the Arduino

## Project Steps

### Understanding The 7-Segment Display

- A 7-segment display is an electronic component used in devices like digital clocks and calculators.

- It consists of seven individually illuminated segments arranged in a specific pattern.

- These segments can be independently turned on or off to display numbers from 0 to 9 and sometimes additional characters.

- When activated in combination, these segments create the desired numeral or character.

- The display is controlled by electronic circuits that determine which segments should be illuminated to represent the desired digit or character.

- Below is an example of a 7-segment display. 

<img src="./assets/7segment.png" alt="7-segment display" />

### The Voltage Divider

#### 1. Understanding the Voltage Divider

- A voltage divider is a fundamental circuit used to generate a specific voltage level from a power supply. Imagine it as a way to adjust the volume of electricity, similar to adjusting the volume knob on a speaker.

<img src="./assets/voltage_divider1.png" alt="voltage divider example" />

- Consider the circuit above. Here we have a single resistor in a circuit that is wired between Vcc and GND. The equation that governs the operation of this circuit is **V = IR** with **V** being the voltage, **I** as the current and **R** is the resistance value of the resistor. 

<img src="./assets/voltage_divider2.png" alt="2 resistors" />

- Now lets look at an example of a voltage divider above. We are having two resistors lining up in one path. The total resistance **R = R1 + R2** would be used to compute the current **I**. 

- Given an electricity current of +5 Volts that flows through the circuit, some voltage is lost at **R1** and the rest is lost at **R2**. The ratio of these resistance values determines the amount of voltage at location **V** as a a fraction of the voltage **Vcc**, which can be calculated like below: 

<img src="./assets/equation.png" alt="equation" />

- By choosing our two resistance values, we can pick any voltage **V** that we desire (between 0 and 5 Volts).

#### 2. Understanding the Potentiometer

#### 3. Wiring the Potentiometer

#### 4. Reading and Converting the Potentiometer Output


### Designing The Combinational Circuit

#### 1. Designing the Logic with Karnaugh Maps 

#### 2. Testing the Logic with **Logisim**


### Putting It All Together

## Testing

## Conclusion




