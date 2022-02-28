# RGB7seg-ShiftBCD
I module to drive an RGB 7 seg 2 digit multiplex lighting display using 4bits BCD+4 bits colour + 2 extra external Red Bits

On SparkFun i found this https://www.sparkfun.com/products/13999
I ordered it and worked through the datasheet - using an ESP32 I wrote a faster shiftOut which is still being tuned
I used 4 bits for the digit which is alternated using the cathode lights on the other 4pins + 2 extra GPIO

This has already evolved into a 2 shift register variant in another project but since I made PCB for this one I decided
to store it's state in this Github repository to help people who may want to do it with TTL logic
