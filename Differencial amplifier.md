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
<b> Aim: design differencial amplifier for following specificationss VDD=2V,p<=1mV,vicm=1V,vocm=1.1V,vp=0.4V perform DC Analysis transient Analysis,frequency responce and exact required parameter<b>
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
To set the operating point go to Configure Analysis and select Dc operating Point and set the Id value


![dc](https://github.com/user-attachments/assets/5a9535dc-0bc8-403b-b05a-ac7a2e35e036)
<br>
Here in dc analysis we got the vout=1.100 as expected and we got the same id1=id2=2.49
<br>
<b> Transient analysis:<b>
<br>
To perform transient analysis we have to select the transient analysis in the edit simulation and give the stop time as 5ms and run the simulation . and the graph velow shows the transient response of the design.


![trans](https://github.com/user-attachments/assets/ab07487e-56bc-4184-98a1-79d8e44b319e)
<br>
voltage gain AV=voutp-p/vinp-p

AV=(1.53-0.63)/(1.08-0.9)

AV=5
<br>
<b> AC Analysis:<b>



![WhatsApp Image 2025-03-04 at 10 12 56 PM](https://github.com/user-attachments/assets/ff5faa5f-7991-4281-b593-6fb8bbdd6056)
<br>
<b> Circuit 2:<b>
<br>
Now replace the R3 resister with a current source : connect a current souce of 0.5mA
<br>
![circuit32](https://github.com/user-attachments/assets/a2268095-2ed0-4ddb-94ce-df0921664902)
<b> DC Analysis:<b>
<br>
To perform the DC analysis we have to select the {DC op pnt} in the edit simulation command and run the simulation the figure below is the values obtained from the DC analysis

![WhatsApp Image 2025-03-04 at 10 27 05 PM (1)](https://github.com/user-attachments/assets/c392b01b-ed40-4954-8d36-3051b28bb197)






