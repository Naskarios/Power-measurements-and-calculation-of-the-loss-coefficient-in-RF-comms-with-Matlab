# Power-measurements-and-calculation-of-the-loss-coefficient-in-RF-comms-with-Matlab

The 2nd lab assignment during the "Wireless Communications" course was about taking measurements and using propagtion models to estimate the power loss in RF communications.Here's how we approached the assignment
## I.Measurements
The measurements  were taken in the corridor outside the lab.The layout of the lab looked similar to the figure below

![qownnotes-media-VZEZhj](https://github.com/Naskarios/Power-measurements-and-calculation-of-the-loss-coefficient-in-RF-comms-with-Matlab/blob/main/qownnotes-media-VZEZhj.png)

In the contex of this lab project we used the __spectrum analyzer__(Aim TTi PSA 6005) to take measurements of the power transimitted by the __RF generator__(Agilent N5182A ) equiped with the Amphenol Procom CXL-1/m __antenna_,the signal generated was a simple cosine signal at __900Mhz__ and the power was set to __-1dbm__ .

The *measurement procedure* went as it follows:
1. The spectrum analyzer started at do distance from the generator,as shown in the figure
2. The analyzer was moved 50cm until it reached the elevator near the lab (the total distance from the generator was around 12.5m).Each time the analyzer was moved,measurements were noted by the students (myself and my colleagues).
3. Then the analyzer and the generator were powered off.
## II.Loss coefficient estimation
By using the minimun square method via the __polyfit()__ function in matlab with the distances from do and the corresponding losses as its arguments,we were able to calculate an estimation for the loss coefficient.

After that we used the coefficient in the model shown below and made our plots.The plots can be viewed by running the Matlab code or from the pdf available ![here](https://github.com/Naskarios/Power-measurements-and-calculation-of-the-loss-coefficient-in-RF-comms-with-Matlab/blob/main/untitled.pdf)


![qownnotes-media-VATNzY](https://github.com/Naskarios/Power-measurements-and-calculation-of-the-loss-coefficient-in-RF-comms-with-Matlab/blob/main/qownnotes-media-VATNzY.png)


|No |	DIST (m) |	RECIEVED POWER(dBm) |
|---|---|---|
|1|	0,5|	-49|
|2 |	1|	-47,2|
|3 | 1,5|	-44,3|
|4 |	2|	-56|
|5|	2,5 |	-68|
| 6 |	3	|-56,5|
| 7 |	3,5	|-59,7|
| 8 |	4	|-61,7|
| 9 |	4,5	|-63|
| 10  |	5	|-59,8|
| 11  |	5,5	|-56|
| 12  |	6	|-71|
| 13  |	6,5	|-73|
| 14| 	7	|-64|
| 15| 	7,5	|-66,4|
| 16| 	8	|-73|
| 17| 	8,5	|-62,1|
| 18	|9	|-67|
| 19	|9,5|	-71|
| 20	|10	|-76,5|
| 21|	10,5|	-67,8|
| 22|	11	|-67|
| 23|	11,5|	-70,5|
| 24|	12	|-73|
| 25|	12,5|	-72,5|




