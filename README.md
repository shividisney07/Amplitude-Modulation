# Amplitude-Modulation

EXP NO: 1	GENERATION AND DETECTION OF AM

AIM:

To generate and detect the amplitude modulation and demodulation u s i n g S C I L A B and to calculate modulation index of AM.

EQUIPMENTS REQUIRED

•	Computer with i3 Processor

•	SCI LAB

THEORY:

Modulation can be defined as the process by which the characteristics of carrier wave are varied in accordance with the modulating wave (signal). Modulation is performed in a transmitter by a circuit called a modulator.
Need for modulation is as follows:
•	Avoid mixing of signals
•	Reduction in antenna height
•	long distance communication
•	Multiplexing
•	Improve the quality of reception
•	Ease of radiation.
Amplitude Modulation is the process of changing the amplitude of a relatively high frequency carrier signal in proportion with the instantaneous value of the modulating signal. The output waveform contains all the frequencies that make up the AM signal and is used to transport the information through the system. Therefore the shape of the modulated wave is called the AM envelope. With no modulating signal the output waveform is simply the carrier signal. Coefficient of modulation is a term used to describe the amount of amplitude change present in an AM waveform. There are three degrees of modulation available based on value of modulation index.
1)	Under modulation :	m<1, Em < Ec
2)	Critical modulation: m-1, Em = Ec
3)	Over modulation:	m>1, Em > Ec



Note: Keep all the switch faults in off position

Algorithm
1.	Define Parameters
First, define the parameters for your signals:
•	Carrier frequency (fc)
•	Modulating signal frequency (fm)
•	Sampling frequency (Fs)
•	Duration of the signal (T)


2.	Create a time vector based on the sampling frequency and duration.
 
3.	Create Modulating Signal
Define the modulating signal (message signal).

4.	Create Carrier Signal
Define the carrier signal.


5.	Perform Amplitude Modulation
Multiply the carrier signal by the modulating signal plus 1 (to ensure the modulation depth).


6.	Plot the Signals
Visualize the modulating, carrier, and modulated signals.


7.	Demodulate the AM Signal
To demodulate, you can use envelope detection. One way is to rectify the signal and then apply a low-pass filter.

8.	Plot the Demodulated Signal
Visualize the demodulated signal.


9.	Compare Signals
Compare the original modulating signal with the demodulated signal. PROCEDURE
•	Refer Algorithms and write code for the experiment.
•	Open SCILAB in System
•	Type your code in New Editor
•	Save the file
•	Execute the code
•	If any Error, correct it in code and execute again
•	Verify the generated waveform using Tabulation and Model Waveform

Program
```
Am=1.68;
Ac=2*Am;
fm=243;
fc=10*fm;
fs=10*fc;
t=0:1/fs:2/fm;
em=Am*cos(2*3.14*fm*t);
ec=Ac*cos(2*3.14*fc*t);
eam=ec.*em;

subplot(3,1,1);
plot(t,em);
subplot(3,1,2);
plot(t,ec);
subplot(3,1,3);
plot(t,eam);
```


Output Waveform
<img width="606" height="478" alt="50d7a00a-6375-4835-a882-a0a21c0e84be" src="https://github.com/user-attachments/assets/6b50a5ee-28b9-45ff-99cc-e15aeb945903" />





TABULATION:

<img width="1600" height="962" alt="dfaeaef7-a5de-48c0-8ddf-609fa91732c6" src="https://github.com/user-attachments/assets/11f6ad4e-489b-49b2-be2e-06e692d69a6d" />


Calculation:

<img width="899" height="1599" alt="42272a2f-dd45-496d-991a-eae2381ff4d1" src="https://github.com/user-attachments/assets/108be5a2-b6dd-4a5b-97bb-6acd30248cc6" />



MODEL GRAPH
 <img width="919" height="1290" alt="image" src="https://github.com/user-attachments/assets/55326c5b-7dd5-4873-aaf6-d219bb7c4420" />

 
 


RESULT:
Thus the amplitude modulation and demodulation is experimentally done and the output is verified.
