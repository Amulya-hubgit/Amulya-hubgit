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




