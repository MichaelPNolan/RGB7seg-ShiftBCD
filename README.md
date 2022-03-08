# RGB7seg-ShiftBCD
I module to drive an RGB 7 seg 2 digit multiplex lighting display using 4bits BCD+4 bits colour + 2 extra external Red Bits
the branch with moar (see below)

On SparkFun i found this https://www.sparkfun.com/products/13999
I ordered it and worked through the datasheet - using an ESP32 I wrote a faster shiftOut which is still being tuned
I used 4 bits for the digit which is alternated using the cathode lights on the other 4pins + 2 extra GPIO

This has already evolved into a 2 shift register variant in another project but since I made PCB for this one I decided
to store it's state in this Github repository to help people who may want to do it with TTL logic

Moar:
To recover 2 GPIO i have a second shift register daisy chained and it is taking the RGBx2 sets as well as 1 pin for a 3rd digit
I've also added a 14 segment 4 digit alphanumeric in the same size as seen here https://www.digikey.com/en/maker/blogs/2022/an-introduction-to-14-segment-led-displays-with-the-ht16k33-driver
That uses i2c

You can repurpose this to show whatever you need 3 digit values + 4 or more (scrolling) of char/text
