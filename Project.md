# TEMPERATURE SENSING AND CONTROLLING


## Group 11: 
            EE23MT017 Sahil Bagade;   EE23MT017@gmail.com            
            EE23Mt008 JAYASURIYA T J  EE23MT008@gmail.com

## Aim: 
            Design a 6 bit 2 step Flash ADC [3 bit + 3 bit]

## Circuit Block Diagram 

 
<img src="Blockdiag.png" alt="Block Diagram" height="550" width="750"/>

    
    
    
## Sub Circuit 
S/H Circuit

<img src="Transmission Gate.png" alt="S/H Circuit" height="450" width="550"/>

3 bit ADC

<img src="3bitADC.png" alt="3bitADC" height="450" width="550"/>

3 bit DAC

<img src="3bitDAC.png" alt="3bitDAC" height="450" width="550"/>



##Challenges 

            S/H Circuit
            
            First the s/h circuit we used was the bottom plate sampling, the problem we faced while using the bottom plate sampling was the output we got was 

            After replacing bottom plate sampling ckt with the transmission gate, at the output, the capacitor was charging slowly when the capacitor of 1u F was connected and there were errors when the
            1f F was connected.

            3 Bit ADC

            3 Bit DAC

            The voltage we got at the nodes was not the same as expected. The problem with our circuit was the mos resistance due to which the division of voltage was not proper, the expected division 
            was Vref/2 , Vref/4 , Vref/8.This problem was rectified by replacing the pmos with nmos and conntecting intvertor to the gate of nmos and its source is connected to ground. So that when the 
            input 0 is given to dac inverted nmos will be turned on and it will be shorted to ground.

            

            


            



## Results:

We have to sense the temperature of a resistor using an LM35 temperature sensor. And we have to control the temperature of a resistor using a switch. 
The  temperature sensing is done by controlling the current in the Temperature sensing module using a switch of the microcontroller, where we have used the LM35 sensor to detect the rise in temperature and sent the data to the microcontroller



