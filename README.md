# ALU-for-8-bit-computer
ALU-for-8-bit-computer
hey, i started this project a long time ago, before joining slack, and left it in the middle, but now, i am rebuilding it. I had already built: clock, program counter, 2 registers. now, i'll be continuing to build it, starting with the ALU. I also hope to build the RAM, control circuit, display, in the coming time

this design is based on the albert paul mavino and ben eater design. It only has addition and subtraction functions because it is a very basic(SAP-1) computer.
please note that connecting wires, each of which is made exactly as long as it needs to be, is a time taking process.so, even if i had added only few wires, it took a long time to do so.

## session 1: 
wired the ALU chips, 74ls283 and 74ls86. 4 bit full adder and 4 XOR gates, to the Registers(A and B). now, internal wiring of ALU is left which is for the next session. some pictures and a video are attached below.

https://github.com/user-attachments/assets/cb9eb938-300b-44e4-9bd2-3a80926242a4

[YT timelapse of build](https://www.youtube.com/watch?v=9lxvixsojeM)
### paperschematic
![pic2](https://github.com/user-attachments/assets/f0a06557-9918-44b0-8bc9-ad49e195a880)


### before

![pic3](https://github.com/user-attachments/assets/cefb166d-0355-49ec-8175-b7a5e0f573ea)
![pic1](https://github.com/user-attachments/assets/629c52e6-ac3b-4b49-8eb0-7719de5cc796)


### after
![pic4](https://github.com/user-attachments/assets/ec9abefd-5234-4e78-922f-3ef6d026b93f)


## session 2:
added all the internal wiring left. Now i dont have any wires left lol. that is why i added a different coloured wire in the last joint. i have to get the blue coloured one from school now lol. next session will be based on checking(and probably troubleshooting) the ALU. here are the images and the videos:

### video(yt)
[YT timelapse of build](https://www.youtube.com/watch?v=6CFhO3uQEqo)

### before
![pic4](https://github.com/user-attachments/assets/ec9abefd-5234-4e78-922f-3ef6d026b93f)

### after
![pic5](https://github.com/user-attachments/assets/4daf0673-32a0-4b5f-aeec-0020deef43fe)


## session3:
in this session, i'll be testing the ALU and writing how it works in detail. 
The ALU is working fine

### video
[YT timelapse of build](https://www.youtube.com/watch?v=xTb6hE4NxM8)

## working
this ALU comprises of 2 74LS283's and 2 74LS86's. the 74LS283 is a full adder and the 74LS86 is the XOR gate ic. The data on register A is always inputted into the ALU, which is the same case for register B but the data from register B is first fed into the XOR gates then the Adders. This is because it is the way to subtract using two's complement. the first input of XOR is from register B and the second is an input called "SUB". when sub is on, all the bits are inverted. and also, SUB is fed into the carry in of the first adder. both the adders are connected by carry. carry out of first is fed into carry in of second. this leads to subtraction of the numbers. and they get added when SUB is turned off. SUB will be controlled by the control lines when the computer is fully built. 

### images
![pic6](https://github.com/user-attachments/assets/4c81ae47-918f-4e9f-9549-55c0ba6b99a5)

![pic7](https://github.com/user-attachments/assets/c0c00995-23ae-4be9-9761-87509a4813f3)

LSB means Least significant bit while MSB means most significant bit. in 10, LSB is 0 while 1 is MSB. in 10111111, MSB and LSB both are 1.
(The output LEDs for the adders are not in LINE as the Registers because i was out of wires so i was not able to connect them to the Buffer IC, 74HC245)
the lines made by me show the decreasing significance of bits. 
That's all. Thank you for reading....
