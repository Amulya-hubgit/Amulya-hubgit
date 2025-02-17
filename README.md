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
<br>.
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
=1/2<b> u<sub> n</b><b> C<sub>ox</b>W/L(<b> V<sub>gs</b>-<b> V<sub>th</b>
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
<b> A<sub> v</b>=-33.48dB
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

![AC](https://github.com/user-attachments/assets/f17c6aff-9b11-4fc5-ad46-2eb5fc3b9137)
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







 
