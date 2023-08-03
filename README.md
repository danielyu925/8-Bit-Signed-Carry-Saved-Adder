# 8-Bit-Signed-Carry-Saved-Adder

<img src="/Figure/Tape_Out_Chip.png">

The carry-save adder is capable of simultaneously calculating the sum of three numbers. It performs the addition of corresponding bits from the three inputs to generate the sum and carry (C) for each bit. Then, it adds the previous carry (C) to the sum of the next bit to obtain the final result of the three-number addition.

<img src="/Figure/Architecture.png">

The design utilizes a Decoder to allocate and share input pins among the three numbers, reducing the number of chip pins from 40 to 32 and consequently minimizing the layout area after adding the PAD.

<img src="/Figure/Layout.png">

The design was implemented using the UMC 0.18 um process, and the fabricated chip was successfully tested and validated using signal generators and oscilloscopes at the school to confirm its proper functionality.
