# 8-Bit Signed Carry Saved Adder
<img src="/Figure/Tape_Out_Chip.png">

## Design Architecture
The numerical input is 8-bit, where the first 7 bits INPUT[6:0] represent the pure numerical value, and the 8th-bit INPUT[7] indicates the sign, with 1 representing negative and 0 representing positive (the numerical input range is from - 127 to +127). The output employs a 10-bit two's complement representation, ranging between -381 and +381.
<img src="/Figure/Architecture.png">


### Carry Save Adder(CSA)
The carry-save adder can simultaneously calculate the sum of three numbers. It adds corresponding bits from the three inputs to generate the sum and carry (C) for each bit. Then, it adds the previous carry (C) to the sum of the next bit to obtain the final result of the three-number addition.
<img src="/Figure/CSA.png">

## Result
The design utilizes a Decoder to allocate and share input pins among the three numbers, reducing the number of chip pins from 40 to 32 and consequently minimizing the layout area after adding the PAD.

The design was implemented using the UMC 0.18 um process, and the fabricated chip was successfully tested and validated using signal generators and oscilloscopes at the school to confirm its proper functionality.

## Layout
<img src="/Figure/layout_no_pad.png">
<img src="/Figure/Layout.png">

## Report
[8-bit Signed Carry Saved Adder Report](CSA_Final_Report.pdf)
