# **Experiment 3**
## **DC,Transient Analysis and AC analysis of Diffrencial Amplifier MOSFET**
### **Introduction:**
A MOSFET differential amplifier amplifies the voltage difference between two input signals while rejecting common-mode noise. It consists of two matched MOSFETs, a current source, and load resistors or an active load. The MOSFETs share a common bias current, which splits between them based on the input voltages.
<br>
In differential mode, if one input voltage increases while the other decreases, the current through one MOSFET rises while the other falls, creating a voltage difference at the output. In common-mode operation, where both inputs change together, the circuit maintains a balanced current flow, minimizing output variation and rejecting noise.
<br>
Applications of Differential amplifiers are widely used in Operational amplifiers (op-amps),Analog-to-digital converters (ADCs),Sensor signal conditioning,Communication circuits (such as mixers and amplifiers) a due to its high common-mode rejection ratio (CMRR), high input impedance, and low distortion.
<br>
<br>
<b> Aim: design differencial amplifier for following specificationss VDD=2V,p<=1mV,vicm=1V,vocm=1.1V,vp=0.4V perform DC Analysis transient  Analysis,frequency responce and exact required parameter<b>
<br>
<br>
<b> Circuit Calculations:<b>


![circuit calu](https://github.com/user-attachments/assets/b1f54767-9178-4202-9511-af3b93569961)
<br>
<b>Circuit Diagram:<b>

![circuit 2](https://github.com/user-attachments/assets/0ade39ad-1907-4b6b-b5bf-67ba6996d515)

<br>
<b> Circuit 1:<b>


![cicuit1](https://github.com/user-attachments/assets/199d3666-d2fa-41ac-880c-30f58605d874)
<br>
Now to get the desired values of output voltage and current we have to vary the width and length of both the mosfet we got Length=180nm and width=19.3um
<br>
<b> DC analysis:<b>
<br>
To set the operating point go to edit simulation and select Dc operating Point in the simulation and set the Id value


![dc](https://github.com/user-attachments/assets/5a9535dc-0bc8-403b-b05a-ac7a2e35e036)
<br>
Here in dc analysis we got the vout=1.100 as expected and we got the same id1=id2=2.49
<br>
Q-point of the mosfet =(0.77,0.25m) at Vgs=0.6
<br>
<b> Transient analysis:<b>
<br>
In transient analysis we have to select the transient analysis in the edit simulation and give the stop time as 3ms and run the simulation . and the below gragh shows the transient response of the design.


![trans](https://github.com/user-attachments/assets/ab07487e-56bc-4184-98a1-79d8e44b319e)
<br>
voltage gain AV=voutp-p/vinp-p
<br>
AV=(1.53-0.65)/(1.03-0.94)
<br>
AV=9.73
<br>
Swing Calculation
<br>
Vinmin=Vth+Vp
<br>
Vinmin=0.36+0.4=0.76V
<br>
Vinmax=Vdd-IdRd+Vth
<br>
Vinmax=2-(0.25m×3.6k)+0.36=1.46V
<br>
i/p max swing=(0.76+1.46)/2 = 1,11V
<br>
Voutmin = Vov+Vp
<br>
Voutmin =(0.6-0.36)+0.4 =0.64
<br>
Voutmax=Vdd-IdRd
<br>
Voutmax=2-(0.25m×3.6k)=1.1
<br>
o/p max swing =(1.1+0.67)/2=0.87

<br>
<b> AC Analysis:<b>



![WhatsApp Image 2025-03-04 at 10 12 56 PM](https://github.com/user-attachments/assets/ff5faa5f-7991-4281-b593-6fb8bbdd6056)
<br>
AV 9.73V/V
<br>
dB=20log(Av)
<br>
dB=20log(9.73)
<br>
dB=19.7
<br>
<b> Circuit 2:<b>
<br>
Now replace the R3 resister with a current source : connect a current souce of 0.5mA
<br>
![circuit32](https://github.com/user-attachments/assets/a2268095-2ed0-4ddb-94ce-df0921664902)
<b> DC Analysis:<b>
<br>
In the DC analysis we have to select the DC operating point in the edit simulation command and run the simulation the figure below is the values obtained from the DC analysis

![WhatsApp Image 2025-03-04 at 10 27 05 PM (1)](https://github.com/user-attachments/assets/c392b01b-ed40-4954-8d36-3051b28bb197)
<br>
Transient Analysis:
<br>
To perform transient analysis we have to select the transient analysis in the edit simulation and give the stop time as 3ms and run the simulation and we get the output waveform
![WhatsApp Image 2025-03-04 at 10 38 49 PM](https://github.com/user-attachments/assets/9ae558c7-48e5-4471-9430-745b7d9fdf43)
<br>
AC Analysis:
<br>

![ac curre1](https://github.com/user-attachments/assets/372e900c-724a-43b7-8165-ad787d11a123)
<br>
<br>
<b> circuit 3:<b>
Now replace the R3 resister with a Mosfet 

![mos](https://github.com/user-attachments/assets/7a377fd3-312b-433d-aad8-941352d3ef06)
<br>
Vb=Vth+Vp
<br>
Vb=0.36+0.4=0.76
<br>
DC Analysis:
![dc mos](https://github.com/user-attachments/assets/044a39ab-82b3-4f0c-865e-cdf9b8ec7531)
<br>
Transient Analysis:
<br>

![trans mos](https://github.com/user-attachments/assets/3ac01651-9175-4e32-8368-f13f674d9cf8)
<br>
AC Analysis:
<br>

![ac mos](https://github.com/user-attachments/assets/bf9f44c9-9dce-4da5-8e15-9b29deecafb3)
<br>
<b> Inference:<b>
<br>
1.In this Experiment we seen the working prinicipal of differencial amplifier and it's types and configurations
<br>
2.when resistor is connected to the differencial amplifier it gives the low CMRR because resistors do not reject common-mode signalss well,low gain due to limited impedence and provide high Bandwidth
<br>
3.Replacing the resistor with a current source as a load significantly improves performance. A current source has high output impedance,This results in high gain and better CMRR, as the current source helps reject common-mode signals.
<br>
4.Replacing the current source with nmosfet it provides very high impedance, leading to maximum gain and excellent CMRR. Active loads are commonly used in integrated circuits (ICs) and operational amplifiers (op-amps) due to their space and power efficiency.
<br>
| Load Type        |    Gain   | output impedence | CMRR    |Complexity|
|------------------|-----------|------------------|---------|----------|
|   Resistor       | low       |     low          |   low   |  simple  |
|   Current souce  | high      |     high         |   high  |  moderate|
|    mosfet        |very high  |    very high     |very high|  complex |











