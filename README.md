# Experiment-08- Encoders-and-decoders 
### AIM: To implement 8 to 3 Encoder and  3to8 Decoder using verilog and validate its outputs
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## Encoders
Binary code of N digits can be used to store 2N distinct elements of coded information. This is what encoders and decoders are used for. Encoders convert 2N lines of input into a code of N bits and Decoders decode the N bits into 2N lines.

1. Encoders –
An encoder is a combinational circuit that converts binary information in the form of a 2N input lines into N output lines, which represent N bit code for the input. For simple encoders, it is assumed that only one input line is active at a time.

As an example, let’s consider Octal to Binary encoder. As shown in the following figure, an octal-to-binary encoder takes 8 input lines and generates 3 output lines.

![image](https://user-images.githubusercontent.com/36288975/171543588-bc0746df-a173-4b35-989e-5fb7d385fe8a.png)
## Figure -01 3 to 8 Encoder 


Implementation –

X = D4 + D5 + D6 + D7
Y = D2 +D3 + D6 + D7
Z = D1 + D3 + D5 + D7 
Hence, the encoder can be realised with OR gates as follows:


![image](https://user-images.githubusercontent.com/36288975/171543740-68403b82-aa93-4c98-9343-f32b14885a2e.png)
## Figure -02 3 to 8 Encoder implenentation 

 ### Decoders 
A decoder does the opposite job of an encoder. It is a combinational circuit that converts n lines of input into 2n lines of output.

Let’s take an example of 3-to-8 line decoder.
Implementation –
D0 is high when X = 0, Y = 0 and Z = 0. Hence,

D0 = X’ Y’ Z’ 
Similarly,

D1 = X’ Y’ Z
D2 = X’ Y Z’
D3 = X’ Y Z
D4 = X Y’ Z’
D5 = X Y’ Z
D6 = X Y Z’
D7 = X Y Z 


![image](https://user-images.githubusercontent.com/36288975/171543978-ee2d0671-2846-40a1-8705-507fd6287a49.png)
## Figure -03 8 to 3 Decoder 



![image](https://user-images.githubusercontent.com/36288975/171543866-5a6eace6-8683-49d7-9c4f-a7cb30ec3035.png)
## Figure -04 8 to 3 Decoder implementation 

### Procedure
/* write all the steps invloved */



### PROGRAM 
/*
Program for Endocers and Decoders  and verify its truth table in quartus using Verilog programming.
Developed by: RAJAGOPAL V 
RegisterNumber: 23002920
*/
### Code 
### ENCODER 
![292669242-4935459f-e3d5-421d-9751-ac618a5e80f3](https://github.com/Rajagopalvengatesan/Experiment-08-Encoders-and-decoders-/assets/144870784/7f7ec72f-6ce9-4363-89ca-3cb3c1593226)

### DECODER 

![292669275-0c3c1120-7c83-482a-a1ca-ef0f541c1223](https://github.com/Rajagopalvengatesan/Experiment-08-Encoders-and-decoders-/assets/144870784/0af0fd31-eeef-458f-93e6-e3c59ce70959)



### RTL LOGIC  
### ENCODER 
![292669293-27485317-6cb8-41f3-9a9a-200e7dc9a14a](https://github.com/Rajagopalvengatesan/Experiment-08-Encoders-and-decoders-/assets/144870784/8c2c6d5d-5b45-4457-ae44-a710e08ad92c)

### DECODER


![292669309-ab63cadc-8a25-4e7c-afef-84142dce209f](https://github.com/Rajagopalvengatesan/Experiment-08-Encoders-and-decoders-/assets/144870784/eac0d2ea-9964-41a9-8b47-57de7e6df903)




### TIMING DIGRAMS  

### ENCODER 

![292669376-fb533307-29bc-40f1-acdc-61f3114c07ad](https://github.com/Rajagopalvengatesan/Experiment-08-Encoders-and-decoders-/assets/144870784/44ff2c71-e7b7-43c2-bf3a-b2004b8c9825)

### DECODER 
![292669389-b4e2be5b-af03-4a8b-9dee-289a79450913](https://github.com/Rajagopalvengatesan/Experiment-08-Encoders-and-decoders-/assets/144870784/00fda088-6ddb-4482-a5fe-7f86cc7360c8)





### TRUTH TABLE 

### ENCODER 

![292669345-6283fa44-f4f0-457f-9221-ab529559c4fe](https://github.com/Rajagopalvengatesan/Experiment-08-Encoders-and-decoders-/assets/144870784/56e2ac67-1469-4e75-b067-9e0192f04934)

### DECODER 
![292669364-8d6ee27f-bce1-448b-9bbc-a7d185c39fa2](https://github.com/Rajagopalvengatesan/Experiment-08-Encoders-and-decoders-/assets/144870784/b11737d5-3139-4542-a82a-faa6982eb98b)

### RESULTS 
