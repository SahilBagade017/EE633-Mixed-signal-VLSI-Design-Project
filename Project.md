# TEMPERATURE SENSING AND CONTROLLING


## Group 11: 
            EE23MT017 Sahil Bagade;   EE23MT017@gmail.com            
            EE23Mt008 JAYASURIYA T J  EE23MT008@gmail.com

## Aim: 
            Design a 6 bit 2 step Flash ADC [3 bit + 3 bit]

## Circuit Block Diagram 

 

Block Diagram

<img src="block" alt="Block Diagram" width="550"/>



 
The Temperature sensor module consists of one resistor and one  LM35 as a temperature sensor.
<img src="images/LM35.png" alt="Tiva" height="350" width="550"/>

    LM35 has three pins:

    PIN 1 : Vcc, it is the input pin (5v)

    PIN 2 : Vout, we get output (it should be connected to the analog pin microcontroller)

    PIN 3 : GND, it is used for ground

    Features: 
    • Calibrated Directly in Celsius (Centigrade)
    • Linear + 10-mV/°C Scale Factor
    • 0.5°C Ensured Accuracy (at 25°C)
    • Rated for Full −55°C to 150°C Range
    • Suitable for Remote Applications
    • Low-Cost Due to Wafer-Level Trimming
    • Operates From 4 V to 30 V
    • Less Than 60-μA Current Drain
    • Low Self-Heating, 0.08°C in Still Air
    • Non-Linearity Only ±¼°C Typical
    • Low-Impedance Output, 0.1 Ω for 1-mA Load
 
TIVA Microcontroller


<img src="images/Tiva.jpeg" alt="Tiva" width="550"/>


BJT


<img src="images/BJT 2N3055.jpeg" alt="Tiva" width="550"/>

<img src="images/BJT Pins.jpeg" alt="Tiva" width="550"/>
    
    
    
## Circuit Diagram
<img src="images/Ckt Diag.jpeg" alt="Tiva" width="750"/>

## Circuit Implementation
<img src="images/Ckt implementation.jpeg" alt="Tiva" width="750"/>

## PWM Signal
<img src="images/PWM.jpeg" alt="Tiva" width="750"/>

## PWM Max Duty Cycle
<img src="images/PWM Max.jpeg" alt="Tiva" width="750"/>

## PWM Min Duty Cycle
<img src="images/PWM Min.jpeg" alt="Tiva" width="750"/>




## Results:

We have to sense the temperature of a resistor using an LM35 temperature sensor. And we have to control the temperature of a resistor using a switch. 
The  temperature sensing is done by controlling the current in the Temperature sensing module using a switch of the microcontroller, where we have used the LM35 sensor to detect the rise in temperature and sent the data to the microcontroller



