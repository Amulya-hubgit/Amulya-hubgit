# current mirror
## Aim:
### Question a]:
Design and analyse the current mirror circuit for the following specifications.
<br>
- Vdd = 1.8V
- Av > -10V/V 
- P <= 1mW
Perform the DC analysis, Transient analysis and AC analysis. ALso find the maximum output swing and bandwidth
<br>
<b> Question b]</b>
<br>
Design the differential amplifier using the same design specification.
<br>
- P <= 2.2mW
  <br>
- Vocm = 1.25V
  <br>
- Vicm = 1.2V
  <br>
- Vp = 0.4V
  <br>
  - Vdd = 2.2V
  <br>
Perform the DC analysis, transient analysis, AC analysis and extract the parameters.
<br>
<b> Theory:</b>
<br>
A current mirror is a circuit that copies or mirrors a reference current (Iref) from one MOSFET to another while maintaining a stable output current (Iout). It is widely used in analog circuits for biasing and as an active load in amplifiers.
<br>



![real curcuit](https://github.com/user-attachments/assets/03480a59-f8b9-4fac-8d45-11a2b550a670)
<br>
The relation between the ID1 and IREF can be given by the following expression.
![current-mirror_4](https://github.com/user-attachments/assets/f437b7c6-fb35-4a98-98c1-6d357b94e9a0)

<br>
M1 and M2 have the same gate to source voltage (Vgs).
If both transistors are identical, they will have the same drain current in saturation:
<br>
<b>Iout=ID1=Id2=Iref</b>
<br>
For a MOSFET in saturation mode the drain current is:
<br>
<b>Id=1/2*un*cox*w/L(Vgs-Vth)^2</b>
<br>
un= Electron mobility,
<br>
cox = Oxide capacitance,
<br>
W/L= MOSFET width-to-length ratio,
<br>
Vth = Threshold voltage.
<br>
Since M1 and M2  have the same Vgs , they ideally have the same current.
<br>
<b><ins>Effect of Channel Length Modulation on Current Mirror</ins></b> <br><br>
If the channel length modulation effect is also considered, then as shown in figure the drain to source voltage (V<sub>ds</sub>) of the MOSFET increases, the drain current also slightly increases. <br><br>
Considering the channel length modulation effect, if VDS of MOSFET M1 changes by ΔVDS then the drain current ID1 also changes to ID1 + ΔID1



![channel](https://github.com/user-attachments/assets/7ec31dfc-a764-4e2d-b7a6-25680e11e5d8)
<br>
<b> Question a]:</b>
<br>
<b> Circuit diagram and calcualtion:</b>
<br>
<b> Case1=1:1 ratio</b>
<br>
![dc 1 ratio](https://github.com/user-attachments/assets/68f7c462-5065-40fc-82fc-72bbeca9e89c)
<br>

Itotal = ( Power / Vdd )
= ( 1m / 1.8 )
= 0.55mA

Iref = Id = ( Itotal / 2 )
= 0.55m / 2
= 0.277mA
<br>
<b> DC Analysis:</b>
<br>
keeping (W/L) of MOSFET M1 and M2 (180n/10u) and varying width of M3 MOSFET to ensure that mosfet working in saturtion region
<br>
![dc](https://github.com/user-attachments/assets/0b40a5ac-f861-42be-870f-38847b57f315)
<br>
<b> Transient Analysis:</b>
![image](https://github.com/user-attachments/assets/ae36e3fa-8e14-4fb8-83fb-1ee5a62a246f)
![image](https://github.com/user-attachments/assets/2b1ac83a-918c-44ff-b630-b7a28592969a)
<br>
<b> AC Analysis:</b>
![image](https://github.com/user-attachments/assets/cfa35259-53cc-4775-954a-606c8b07a0db)
Av = 29.02dB.
<br>
bandwidth frequency = 652.698MHz.
<br>
<b> For Length=150nm</b>
<br>
<b> DC Analysis:</b>


![dc5](https://github.com/user-attachments/assets/f67b6bda-f9d3-4627-bb73-99f9d5cc4e47)
<br>
<b> Transient Analysis:</b>
![image](https://github.com/user-attachments/assets/461ca2ca-c02c-4f10-9ee4-4c6b15846a44)
<br>
<b> AC analysis:</b>
![image](https://github.com/user-attachments/assets/c4e65c62-c153-41cd-88e3-9a82ddbef5e7)
<br>
<b> for Length =1um
<br>
<b> DC Analysis:</b>


![Capture](https://github.com/user-attachments/assets/3b01d044-2583-4b86-8b00-9f67c89b3197)
<b> AC Analysis:</b>
![image](https://github.com/user-attachments/assets/4eab987c-112a-46cb-870e-b6bfed04e35a)
### Comparison Table

| Length (L) | Width (W1) | Width (W2) | Width (W3) | Iref | Iout | Vout |
|-----|----|----|----|----|----|-----|
| 180nm | 10um | 10um | 32.4256um | 0.277mA | 0.277mA | 1.00553V |
| 500nm | 10um | 10um | 67.646um | 0.277mA | 0.2777mA | 0.707924V |
| 1um | 10um | 10um | 96.472um | 0.277mA | 0.277mA | 0.337052V |
<br>
<b>  for 1:2 ratio</b>
<br>
for Length=180nm
<br>
<b> Circiut diagram:</b>



![dia2](https://github.com/user-attachments/assets/a3bba894-d151-473c-ab4c-ebd51e22f5b1)
<br>
<b> DC Analysis:</b>


![dc 2](https://github.com/user-attachments/assets/ea77dab2-e943-40b2-9a62-dd1f9b6704ae)
<br>
<b> Transient Analysis:</b>
![image](https://github.com/user-attachments/assets/0bc55641-2b62-4568-98f5-85d610400a56)
<br>
![image](https://github.com/user-attachments/assets/9ff808d6-5cb0-42c4-9f59-31cc0406e122)
<br>
<b> AC analysis:</b>
![image](https://github.com/user-attachments/assets/71729ae8-bc6f-45e8-91cb-0310c07c6597)
<br>
<b> for Length=500nm </b>
<br>
<b> Dc Analysis:</b>

![dc 500](https://github.com/user-attachments/assets/a8438a19-dd5b-4501-aece-2c5e514adf86)
<br>
<b> transient Analysis:</b>

<br>
<b> Ac Analysis:</b>

![ac 500](https://github.com/user-attachments/assets/802adc33-cdf3-46b1-bfff-848a21c2ae28)
<br>
<b> for Length=1um</b>
<br>
<b> DC Analysis</b>

![dc  1u](https://github.com/user-attachments/assets/fe0d603c-f3fa-4a09-a252-f8c7464635ae)
<br>
<b> Transient Analysis:</b>

![tra 500](https://github.com/user-attachments/assets/e007a07c-aa9d-4d8f-996b-a9dba3c4b06a)

<br>
<b> Ac Analysis:</b>

![ac 5001](https://github.com/user-attachments/assets/ba92ab78-2354-4ad6-8fcc-cbe18f845de1)
<br>
### Comparison Table

| Length (L) | Width (W1) | Width (W2) | Width (W3) | Iref | Iout | Vout |
|-----|----|----|----|----|----|-----|
| 180nm | 10um | 20um | 42.833um | 0.185mA | 0.370666mA | 1.03657V |
| 500nm | 10um | 20um | 89.342um | 0.185mA | 0.37066mA | 0.802448V |
| 1um | 10um | 20um | 126.357um | 0.185mA | 0.3706mA | 0.493025V |
<br>
### Case 3: For 2:1 ratio
<br>
<b> Circuit diagram:</b>




![ratio2](https://github.com/user-attachments/assets/a4b60b4f-d7a3-4c10-a1c7-4d5b5b481987)








