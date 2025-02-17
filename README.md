# **Report on DC,Transient analysis and AC analysis of a Common Source Amplifier**
## **Introduction:**
</p>     In this experiment we do the the analysis of common source amplifier 
and common source amplifier is the one used widely in the mosfet amplifier and it gives the 
high voltage gain and it's applications are audio amplifier, signal processing and communication circuits
<br> In this Experiment we do the DC,Tranisient analysis and AC analysis.
dc.<br>
<b> DC Analysis:</b>
In this analysis we determines the biasing point(Q-point) of the MOSFET and ensuring it operates in the saturation region.
<br>
<b> Transient analysis:</b>
In this analysis we determines the time domain responce by varying input signal.
<br>
<b> AC analysis:</b>

In this Analysis we determines gain,input(or)output impedence ,frequency responce and bandwidth.
<br>
<br>
<b style="font-size: 27px;"> Circuit Diagram </b>


 ![Screenshot (600](https://github.com/user-attachments/assets/5ec39989-0a30-4e1b-921d-a3b359814ff9)
<br>
<b> Components:</b>
In this circuit we use 180nm of NMOSFET and Drain resistor and voltage source(V1,V2).
<br>
<b> Circuit Specifications:</b>
 <br>
 <b>MOSFET length:</b>
180nm
<br>
<b> MOSFET Width:</b>
0.321um
<br>
<b> Drain Resistor:</b>
2.72k ohm
<br>
<b> Supply Voltage:</b>
1.8V
<br>
<b> Threshold Voltage:</b>
0.36V
<br>
<b> voltage:</b>
0.9V
<br>
<b> Amplitude and Frequency:</b>
50mV, 1kHz
<br>
<b> procedure:</b>
<br>
1.first we design the circut in LT spice then we do the DC analysis, AC analysis and transient analysis
<br>
2. DC analysis: In DC analysis  we give the value for width=3um and length=180nm of the MOSFET and supply voltage is 1.8 and Vgs =0.9 and we select(.op pnt) and run the circuit
<br>
 3.Transient analysis:In Transient analysis we select the sine wave of the input with amplitude 50mV and frequency 1kHz and we give the stop is 3ms and select the (.tran 3m) to run the program
<br>
  4.AC analysis : In AC analysis select the sweep as decade and give frequency as 0.1KHz to 1THz.AC input is a small signal sine wave, and the gain is measured as the ratio of output peak voltage to input peak voltage and use the commant to run.(.ac dec 20 0.1 1T)
<br>
<b>simulations result and Calculations:</b>
<br>
<b> DC Analysis:</b>
<br>




![dia](https://github.com/user-attachments/assets/c99f2146-840e-49da-b01d-e8e4990a16a0)
<br>


![dc](https://github.com/user-attachments/assets/230737ba-c4c2-45a3-8916-d650cf94fd77)
<br>
From the DC analysis
<br>
<b>V<sub>in</b>
=0.9V
<br>
<b>V<sub>out</b>
=1.649V
<br>
To find <b> I<sub> D </b>
<br>
If the power dessipation is 100um across the resistor and voltage is 1.8V
<br>
power=V*I
<br>
I=power/Voltage
<br>
  =100um/1.8V
  <br>
 =55.5um
<br>
The output load line equation is
<br>
<b> V<sub>out</b>
=<b>V<sub>DD</b>-<b> I<sub> D </b>*<b> R<sub> D </b>
<br>
<b> R<sub> D </b>=(1.8-1.64)/55.5u
<br>
=2.72k ohms
<br>
<b> I<sub> D </b>
=1/2<b> u<sub> n</b><b> C<sub>ox</b>W/L(<b> V<sub>gs</b>-<b> V<sub>th</b>)
<br>
<b> I<sub>D</b> &prop; W
<br>
when we replace the value of drain resistor is 2.75k ohms, then  calculated current value does not match the simulated value and fixed the mosfet length value at 180nm and
vary the width to get exact current value
<br>
| Length   | width    | Id       |
|----------|----------|----------|
| 180nm    | 1um      | 0.000144083 |
| 180nm    | 0.1um    | 1.12775e-05|
|180nm     | 0.2um    | 3.75606e-05|
|180nm     | 0.3um    |  5.25619e-05|
| 180nm    | 0.321um   |  5.55657e-05|
<br>
<b> V<sub> DS</b>=<b>V <sub> D </b>-<b>V <sub> s </b>
<br>
  =0
<br>
<b> V<sub> ov </b>=<b> V<sub> gs</b>-<b> V<sub> th </b>
<br> 
0.9-0.36=0.54
<br>
<b> V<sub> DS </b>><b> V<sub> GS </b>-<b> V<sub> th </b>
<br>
 This analysis confirmed that NMOS operates in saturation region
 <br>
 <b> Transient Analysis:</b>
 <br>
 

 
![trans](https://github.com/user-attachments/assets/0f7158ef-92ca-4150-a70c-1e0bf359651c)
<br>
In this ananlysis we determines the gain.to obtain the sinusoidal voltage signal put peak to peak value is 50mV and frequency is 1kHz and Ac amplitude is 1v and select the stop time 3ms
<br>
The voltage gain is calculated as:
<br>
Gain =<b> V<sub> out</b>/<b> V<sub> in</b>
<br>
<b> A<sub> v</b>=33.48dB
<br>
this value matches the theoritical value which is calculated by:
<br>
<b> A<sub> v</b>=<b> G<sub> m</b><b> R<sub> d</b>
<br>
The output waveform is an amplified and inverted version of the input.
A 180° phase shift is observed in the ouyput.
The circuit amplifies without severe distortion, confirming MOSFET operation in saturation.
<br>
<b> AC Analysis:</b>
<br>

![156](https://github.com/user-attachments/assets/1a40a478-ba45-4e37-9de9-cbe7f0c100e9)

<br>
In this analysis we determines the frequency responce and In  simulation we set the sweep to decade and put staring frequency is 1Hz and stop frequency is 1THz
<br>
At low frequency , the amplifier maintains the  high voltage gain and as frequency increses thre gain starts to decresing due to internal MOSFET capacitance
<br>
<b>Result:</b>
<br>
In DC analysis theoritically we calculated Id value is 55.5um and from the load line we calucated Rd =2.72k ohm
<br>
In Transient analysis we calculated and obtained the gain is -33.48 dB
<br>
In AC analysis 
<br>
<b> Inference:</b>
<br>
<b>DC Analysis :</b>
In dc analysis we  determine the biasing point (Q-point)and we confirm that MOSFRT operates in the saturation region
<br>
<b> Transient Analysis :</b>
Common source amplifier amplifies the 1kHz,50mV input signal and  gain is 15 and 180 degree phase shift at the output.
<br>
<b>AC Analysis :</b>
The frequency sweep from 0.1Hz to 1THz shows that beyond a certain frequency the amplifier loses its ability to amplify effectivily.
and at low frequency it gives the high gain .
<br>
<br>
# Circuit 2
<br>
## Circuit Diagram: 
<br>



![circuit 2](https://github.com/user-attachments/assets/6119c0aa-703b-4d5b-985e-380fd8a92b51)
<Br>
<b> circuit components:</b>
<br>
In this circuit we use 180nm of NMOSFET and instead of drain resistor we replace the 180nm of MOSFET and voltage source(V1,V2).
<br>
<b> procedure:</b>
<br>
1.first we design the circut in LT spice then we do the DC analysis, AC analysis and transient analysis
<br>
2. DC analysis: In DC analysis  we give the value for width=3um and length=180nm of the MOSFET and supply voltage is 1.8 and Vgs =0.9 and we select(.op pnt) and run the circuit
<br>
 3.Transient analysis:In Transient analysis we select the sine wave of the input with amplitude 50mV and frequency 1kHz and we give the stop is 3ms and select the (.tran 3m) to run the program
<br>
  4.AC analysis : In AC analysis select the sweep as decade and give frequency as 0.1KHz to 1THz.AC input is a small signal sine wave, and the gain is measured as the ratio of output peak voltage to input peak voltage and use the commant to run.(.ac dec 20 0.1 1T)
<br>
<b>Simulations Result and Calculations:</b>
<br>
<b> DC analysis:</b>
<br>
![image](https://github.com/user-attachments/assets/0aee3c28-1bcf-4e39-8fb7-bf1eb1344af4)
<br>
<br>
From the DC analysis
<br>
<b>V<sub>in</b>
=0.9V
<br>
<b>V<sub>out</b>
=0.849157
<br>
To find <b> I<sub> D </b>
<br>
If the power dessipation is 100um across the resistor and voltage is 1.8V
<br>
power=V*I
<br>
I=power/Voltage
<br>
  =100um/1.8V
  <br>
 =55.5um
 <br>
 we have to get the output current, Id for the given circuits by adjusting the values of Length & Width of both the MOSFETS M1 & M2 
 <br>
 | Length    | width    | Id         |
 |---------- |----------|----------  |
 | 180nm     | 1um      | 0.00014408 |
 | 180nm     | 0.1um    | 1.27955e-05|
 | 180nm     | 0.2um    | 3.75606e-05|
 | 180nm     | 0.31um   |  5.3289e-05|
 | 180nm     | 0.321um  | 5.55256e-05|
<br>
 <b> Transient analysis:</b>
 <br>
 ![transieby](https://github.com/user-attachments/assets/3c2dfbc1-7e93-41ef-b662-e6b3b5d4c868)

 <br>
  We give a frequency 1kHz and give input as sine wave and 50mV peak amplitude and 0.9V DC offset was applied.The output peak voltage was measured as 1.751V of the sine wave.There is 180 degree phase shift between input and output or the DC level shift.
  <br>
  <b> AC analysis:</b>
  <br>
 
  <br>![c3](https://github.com/user-attachments/assets/bc0e0bf2-a866-435b-8914-92d513f3d866)

   The circuit shows a gain of 14dB and    Frequency: 23.614G Hz.
   <br>
   <b> Inference:</b>
   <br>
   1.The Current Id is dependent on width and hence it changes when the width changes whereas the remaining parameters remain constany.
   <br>
   2.DC operating point analysis cofirmed that the MOSFET operates in saturation region. The observed drain voltage (1.18V) and the drain current(55uA) align with theoretical values.
   <br>
   3.Transient analysis verified that the circuit amplifies the input 1k Hz sine wave with minimal distortion.There is 180 degree phase shift between input and output or the DC level shift.
   <br>
   4.In AC analysis we determine the frequency response by applying the small signal analysis to the circuit . We do this analysis to check in which frequency the circuit acts as the linear amplifier.
   
   


 









 
