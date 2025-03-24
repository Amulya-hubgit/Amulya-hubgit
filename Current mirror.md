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
<br>
<b> DC Analysis:</b>


![dc21](https://github.com/user-attachments/assets/e83f2840-cea4-43cc-9c52-dbf09e825774)
<br>
<b> Transient Analysis:</b>
![trans21](https://github.com/user-attachments/assets/be423102-22c1-4155-a310-2e9313d4fa83)
<br>
<b> AC analysis:</b>
![ac 21](https://github.com/user-attachments/assets/69b89a63-90b1-4d74-b628-92bb0d2e9c3b)
<br>
<b> for length= 500nm</b>
<br>
<b> DC Analysis:</b>
<br>
![dc 5n](https://github.com/user-attachments/assets/704619c8-43d5-4748-bd11-6e775b8c8d52)
<br>
<b> Transient Analysis:</b>
<br>

![tran5n](https://github.com/user-attachments/assets/efd5365b-7b47-4671-8f5e-3e9f233c50da)
<br>
<b> AC analysis:</b>
<br>
![ac5n](https://github.com/user-attachments/assets/4abe0782-b010-4a66-9285-0f2e8b59a62b)
<br>
<b> for length= 1u</b>
<br>
<b> DC Analysis:</b>

![dc 11u](https://github.com/user-attachments/assets/2f91e659-e635-4202-93d1-1bdf79c91963)
<br>
<b> Transient Analysis:</b>
<br>
![trans 1u](https://github.com/user-attachments/assets/27a99f97-6941-454b-beb9-b5554d0a2c6b)
<br>
<b> AC analysis:</b>
<br>
![ac1 1u](https://github.com/user-attachments/assets/d95a4976-403b-44f6-8f87-f6d0e4b2f067)
<br>
### Comparison Table

| Length (L) | Width (W1) | Width (W2) | Width (W3) | Iref | Iout | Vout |
|-----|----|----|----|----|----|-----|
| 180nm | 20um | 10um | 20.75um | 0.1854mA | 0.278mA | 1.0927V |
| 500nm | 20um | 10um | 44.508um | 0.1854mA | 0.2776mA | 0.828632V |
| 1um | 20um | 10um | 62.383um | 0.185mA | 0.278mA | 0.613212V |
### Case 4:  1:3 ratio
<b> Circuit diagram:</b>



Id = $P/Vdd$ = $1m/1.8$ = 0.556mA
 Itotal = Id + 3Iref = 4Iref
   
   Iref = $Id/4$ = $0.556m/4$ = 0.139mA
   <br>
<b> DC Analysis:</b>
![image](https://github.com/user-attachments/assets/f67816ef-b39c-4290-88c9-0b53756d875c)

<br>
<b> Transient Analysis:</b>
<br>
![image](https://github.com/user-attachments/assets/01f2c478-96ce-4cdb-9aa2-c65fa9012538)
<br>
<b> AC analysis:</b>
<br>
![image](https://github.com/user-attachments/assets/82cdd49f-adf2-451a-b62e-0d05c00e02c1)
<br>
<b> for length= 500nm</b>
<br>

<b> DC Analysis:</b>
<br>
![dc 500nm](https://github.com/user-attachments/assets/307eb70a-b2f6-4fd1-8415-27b84f1723af)
<br>


<b> Transient Analysis:</b>
<br>

![trans 500n](https://github.com/user-attachments/assets/079351b9-b0ab-487d-b4e4-f005b84e2cc4)
<br>

<b> AC analysis:</b>
<br>
<br>![ac 500nm](https://github.com/user-attachments/assets/eb081492-e18c-401e-8948-d046a87b82be)
<br>
<b> for length= 1u</b>

<br>

<b> DC Analysis:</b>
<br>


![dc1111111u](https://github.com/user-attachments/assets/fabf92cd-4d8a-4b31-8e28-adff1d0cf79f)
<br>


<b> Transient Analysis:</b>
<br>
![trans111111u](https://github.com/user-attachments/assets/e09026b4-a701-49f6-abf3-d38aaa063a61)
<br>

<b> AC analysis:</b>
<br>

![ac11u](https://github.com/user-attachments/assets/23a5f81a-7168-41e1-9dbd-fca940020691)
<br>
### Comparison Table

| Length (L) | Width (W1) | Width (W2) | Width (W3) | Iref | Iout | Vout |
|-----|----|----|----|----|----|-----|
| 180nm | 10um | 30um | 47.5885um | 0.139mA | 0.417mA | 1.07078V |
| 500nm | 10um | 30um | 99.26um | 0.139mA | 0.417mA | 0.913457V |
| 1um | 10um | 30um | 139.553um | 0.139mA | 0.4166mA | 0.694508V |

### <ins> Circuit b] 
### CIRCUIT DESIGN AND CALCULATIONS:
### Case1 =1:1 ratio
## circuit diagram
![image](https://github.com/user-attachments/assets/15114ca8-bef2-4c26-8674-3a5ec83306e9)
<br>
<b> DC Analysis:</b>
![image](https://github.com/user-attachments/assets/ecc182e4-2759-44b9-8fcc-62c27c651db2)





















