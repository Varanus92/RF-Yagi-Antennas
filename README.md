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

Dipole/fidder - simulation:
![](pic/dipole_only.png)


S11 graph:
![](pic/s11_feeder.png)


Radiation Pattern: 

Logritmic:
![](pic/feeder.png)

Linera:
![](pic/feeder_linear.png)

now i started to build the actual Yagi by adding reflctors and feeders,
to understand the distance between the reflectors,feeder and director, i have used this guide :

![](pic/Antena_configuration.png)

the guide above was taken from the book:
"Antenna Theory Analysis and Design Cropped fixed Constantine A Balanis 2nd Ed John Will"

after adding the reflector i could see big improvment of the S11 and radiation pattern (about X4 times improvment - the reflector concentrate the power wasted in the unwanted directions),the improvment increase while adding each of the directors.
here the final picturs of the Yagi:  

Yagi simulation:
![](pic/yaggi_sim.png)

S11 graph :
![](pic/s11_Yaggi.png)


Radiation Pattern logritmic and linera:
![](pic/rp_Yaggi.png)

![](pic/rp_L_Yaggi.png)



Magnetic and Electric field sections:

Electric:
![test](pic/E_field.png)


Magnetic:
![](pic/M_field.png)



Impedance: (yes...its complex)

![](pic/Impedance.png)







see the incredible enhancment in the directivity and gain!


--------

Now its time to build the actual Yagi:
first i have built the feeder and made sure it deliver the signal at the requested frequency (1800Mhz)

![](pic/feeder_test.png)






after that i have build the actual Yagi - for this picture i am grateful to Tal Yehuda that allowed me to use his :

![](pic/Yaggi_build.png)





in the test itself i have transmitted at 1800Mhz from my anntena and saw on the  received signal - amplitude and freuency.

![](pic/Test.png)
























