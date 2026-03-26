# EC1421-19EC421-Analysis-and-Design-of-Analog-ICs
# DESIGN OF ACTIVE LOW PASS,HIGH PASS AND BAND PASS FILTERS USING OP-AMP 

## AIM: 

To design and obtain the frequency response of 
i) First order Low Pass Filter (LPF) 
ii) First order High Pass Filter (HPF) 
iii) Band pass filter
 
## APPARATUS REQUIRED

<img width="625" height="170" alt="image" src="https://github.com/user-attachments/assets/900fc8b3-3a8c-4208-bf52-98cc9e281e21" />

## THEORY
## LOW PASS FILTER 
 A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 
Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain 
decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain 
rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in 
frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this 
frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB 
frequency, break frequency, or corner frequency.
# HIGH PASS FILTER 
The frequency at which the magnitude of the gain is 0.707 times the maximum value of 
gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band 
frequencies with the highest frequency determined by the closed –loop band width all of the op
amp. 
# BAND PASS FILTER 
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > 
fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass 
filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if 
its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band 
pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of 
band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM: 
## LOW_PASS
<img width="1350" height="1026" alt="image" src="https://github.com/user-attachments/assets/ba5afda7-5f02-40ce-a71a-dd0ce3e0eb55" />

## HIGH-PASS
<img width="1283" height="757" alt="image" src="https://github.com/user-attachments/assets/cea4d33e-9b5f-44f3-a50a-10e401643bcb" />
## BAND-PASS
<img width="1600" height="872" alt="image" src="https://github.com/user-attachments/assets/90633193-e32a-49e1-80aa-5a385a0b55c1" />

## MODEL GRAPH:
## LOW_PASS
<img width="1587" height="1600" alt="image" src="https://github.com/user-attachments/assets/824db2f6-3298-4edc-a791-823de672eb61" />

## HIGH-PASS

<img width="1600" height="1451" alt="image" src="https://github.com/user-attachments/assets/2bba90bb-4e27-4f46-b459-c823ea9a91b7" />


## BAND-PASS
<img width="1561" height="1600" alt="image" src="https://github.com/user-attachments/assets/a42ae998-fab1-495b-8128-044e3c84135b" />

## PROCEDURE - (LPF & HPF): 
1. Connect the circuit as shown in the circuit diagram. 
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. 
select the value of R1 & Rf depending on desired passband gain Af.. 
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
4. Tabulate the output voltage Vo with respect to different values of input frequency. 
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to  get approximately the same characteristic as shown in the model graph. 
# PROCEDURE:BAND PASS FILTER 
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given 
frequencies. 
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF 
followed by a LPF (i.e) HPF in series with LPF. 
3. Connect the circuit as shown in the circuit diagram. 
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
5. Tabulate the output voltage Vo with respect to different values of input frequency. 
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to get approximately the same characteristic as shown in the model graph

## DESIGN:LPF & HPF:

<img width="429" height="324" alt="image" src="https://github.com/user-attachments/assets/b0f0ac0a-3006-494c-9096-e91ae2d6e87c" />

# DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4.  
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency 
of HPF as fL = 1 KHz.  
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf.  
Let C = 0.1μf.  
3. Calculate R from the expression.  
Given: fH = 2KHz  = 1/ (2πR1C1) 
   Let C1 = 0.1 µF, R1 = 7.9 KΩ 
Given: fL = 400Hz  = 1/ (2πR2C2) 
   Let C2 = 0.1 µF, R2 = 39.8 KΩ 
  Pass band Gain=4 
   Now   Ao = 1 + (Rf / R1)  
               2-1=(Rf / Ri) 
                Ri = Rf 
                 Let  Ri = Rf = 10 KΩ
## TABULATION:
## LOW_PASS
<img width="939" height="1519" alt="image" src="https://github.com/user-attachments/assets/32d0740b-636b-4ea6-93d8-3d7a99346c6d" />

## HIGH-PASS
<img width="956" height="1299" alt="image" src="https://github.com/user-attachments/assets/93c07b27-1b1c-4823-9f84-c0339eceae86" />

## BAND-PASS
<img width="934" height="1452" alt="image" src="https://github.com/user-attachments/assets/0f962c9f-c41e-47f4-8619-18daec154f38" />

## GRAPH:
## LOW_PASS
<img width="1376" height="994" alt="image" src="https://github.com/user-attachments/assets/12cce26a-94f4-4e2b-8738-aa242b48668f" />

## HIGH-PASS
<img width="1362" height="1004" alt="image" src="https://github.com/user-attachments/assets/335adf51-3a2f-473a-972a-004e5530b476" />

## BAND-PASS
<img width="1438" height="1066" alt="image" src="https://github.com/user-attachments/assets/21064160-85ac-4f5f-81c5-fae7c37931d0" />

 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

