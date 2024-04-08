# Mixed Signal VLSI Design


## Group  
            EE23MT011 Kaushik Powar; EE23MT011@iitdh.ac.in
            EE23MT017 Sahil Bagade;  EE23MT017@iitdh.ac.in            
            

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

                        Latch

<img src="comparator.png" alt="3bitDAC" height="450" width="550"/>

                        Comparator

<img src="sense.png" alt="3bitDAC" height="450" width="550"/>


## Challenges 

            S/H Circuit
            
            First the s/h circuit used was the bottom plate sampling, the problem with using the bottom plate sampling was the output had error due to charge injection.

            After replacing bottom plate sampling ckt with the transmission gate, at the output, the capacitor was charging slowly when the capacitor of 1u F was connected and there were errors when the
            1f F was connected and the noise was getting introduced.

            The second S/H circuit is used to reduce the noise of the substractor output.
            
            The clk in second s/h is delayed by 1.7n.

            Finally the S/H circuit used was Bottom plate sampling beacuse the practically transmission gate are not used and other s/h circuits are preferred.

            Differential Amplifier

            The problem with the differential amplifier was the gain we were getting was different for different inputs.
            This problem was solved by replacing the differential amplifier with the ideal with the gain of 4.

            3 Bit ADC
            
            Initially we took 14um/28um mosfet width which gave an error while testing, we reduced it to 1um/2um.
            Sense comparator was introducing kickback noises in ADC Vref level therefore preamplifiers were added in the circuits
            The pre amp that was near to the ground was giving errors because they were nmos preamps , so we replaced preamps near ground with pmos preamps
            
            
            3 Bit DAC

            The voltage we got at the nodes was not the same as expected.First we used nmos and pmos in parallel, The problem with that circuit was the mos resistance  which was hard to compaensate
            ,due to which the division of voltage was not proper, the expected division was Vref/2 , Vref/4 , Vref/8.This problem was rectified by replacing the switch with two nmos in parallel and 
            conntecting inverter to the gate of nmos and its  source is connected to ground. So that when the input 0 is given to dac inverted nmos will be turned on and it will be shorted to ground.

            Ideal opamp was implemented using IcVs





            

            


            








