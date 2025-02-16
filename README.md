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

 





 
