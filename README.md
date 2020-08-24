# RF-Yagi-Antenna
## Intro  
A Yagi–Uda antenna, commonly known as a Yagi antenna, is a directional antenna consisting of multiple parallel elements in a line, usually half-wave dipoles made of metal rods.Yagi–Uda antennas consist of a single driven element connected to the transmitter or receiver with a transmission line, and additional "parasitic elements" which are not connected to the transmitter or receiver: a so-called reflector and one or more directors.It was invented in 1926 by Shintaro Uda of Tohoku Imperial University, Japan, with a lesser role played by his colleague Hidetsugu Yagi. (Wikipedia)

## Goal
Design a Yagi antenna with 10 DBi Gain at frequency 1800 Mhz. 
make use of CST Studio Suite , and comparethe result with a realalistic one you have build.

## Solution:
Using CST Studio Suite,
first i designed the feeder, for that - calculate Lambda for the given frequency -Lambda=c/f 
i have added the cilinder,brick,contacts,generator,
at first i didn get the accurate frequency for the S11 graph so i did an optimization - the feeder is complet
here are some graph:
![](s11_feeder.png)

S11 graph 
![](s11_feeder.png)


Radiation Pattern logritmic and linera
![](feederr.png)
![](feeder_linear.png)

now i started to build the actual Yagi by adding reflctors and feeders,

to understand the distance between the reflectors,feeder and director, i have used this guide :

![](Antena_configuration.png)
the guide above was taken from the book:
"Antenna Theory Analysis and Design Cropped fixed Constantine A Balanis 2nd Ed John Will"

after adding the reflector i could see big improvment of the S11 and radiation pattern (about X4 times improvment - the reflector concentrate of power wasted in the unwanted directions),the improvment increase while adding each of the directors.
here the final picturs of the Yaggi:  

S11 graph 
![](s11_Yaggi.png)


Radiation Pattern logritmic and linera
![](rp_Yaggi.png)
![](rp_L_Yaggi.png)


see the incredible enhancment in the directivity and gain!





















