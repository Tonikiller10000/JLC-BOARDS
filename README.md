# JLC1
 
 ### Description:
 This is the first set of boards ordered for personal projects. 
 It contains: a sensor bar for a line follower, a FE1.1s USB HUB, an CH340G FTDI Programmer, an ATmega32U4 microcontroller, an ATmega16U2 microcontroller, an AT90USB162 microcontroller, an eeprom programmer and some side testing boards.


OnBoardd modules:  


- [Sensor Bar (used for the finefollower)](https://github.com/Tonikiller10000/8BitProcessor/tree/main/Processor_ALU_V1.0)
- [FE1.1s USB HUB](https://github.com/Tonikiller10000/8BitProcessor/tree/main/DisplayRegister)
- [CH340G FTDI Programmer](https://github.com/Tonikiller10000/8BitProcessor/tree/main/ClkPulseGenerator)
ATmega32U4 microcontroller
ATmega16U2 microcontroller
AT90USB162 microcontroller
eeprom programmer
and some side testing boards





<table>
  <tr>
    <td><img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(6).png"/></td>


  </tr>
 </table>



<img src="https://github.com/Tonikiller10000/JLC1/blob/main/JLC1_Pictures/JLC1p1.png"/>
<img src="https://github.com/Tonikiller10000/JLC1/blob/main/JLC1_Pictures/JLC1R_F.jpg"/>
<img src="https://github.com/Tonikiller10000/JLC1/blob/main/JLC1_Pictures/JLC1v1.png"/>
<img src="https://github.com/Tonikiller10000/JLC1/blob/main/JLC1_Pictures/JLC1R.jpg"/>
<img src="https://github.com/Tonikiller10000/JLC1/blob/main/JLC1_Pictures/JLC1RB.jpg"/>
<img src="https://github.com/Tonikiller10000/JLC1/blob/main/JLC1_Pictures/JLC1s1.jpg"/>
<img src="https://github.com/Tonikiller10000/JLC1/blob/main/JLC1_Pictures/JLC1s2.jpg"/>
<img src="https://github.com/Tonikiller10000/JLC1/blob/main/JLC1_Pictures/JLC1v3.jpg"/>









### How to use:
1. Put values in the A and B register by putting a value on the bus and setting the A_IN or B_IN pin HIGH.
2. By setting the SUB pin LOW (default), the ALU adds the A Reg value and the B reg Value upt to 255, 
after witch the carry flag gets activated and the result remain the difference between the result and 256.
EX. 199 + 69 = 22(+C)
When the SUB pin is pulled HIGH, the ALU returns the difference between A register value and B register value.
3. The carry input can be changed from the C_IN pin.
4. By setting the F_IN pin HIGH, the flag values are saved in the Flag register. 
5. The result of the ALU can be outputed in the bus by putting the ALU_OUT pin HIGH.
The ALU result can be put back in the A or B registers and be used for other operations.

<table>
  <tr>
    <td><img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(18).jpg"/></td>
    <td><img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(11).jpg"/></td>
    <td><img src="https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(12).jpg"/></td>
  </tr>
 </table>





### Mentions:
- All the pins should have an pull-down resistors to assure the default mode opperation
- By not using resistors for the led\`s thinking that the 74LSx series IC\`s has integrated resistors, the led\`s are to brigth, and their intensity changes depending on how many led\`s are ligthned up. ( https://github.com/Tonikiller10000/8BitProcessor/blob/main/Processor_ALU_V1.0/ALU-Pictures/ALU_Picture%20(17).jpg )
- This is the first version, Future versions will come in the next version of the processor. ( https://github.com/Tonikiller10000/8BitProcessor/tree/main )


