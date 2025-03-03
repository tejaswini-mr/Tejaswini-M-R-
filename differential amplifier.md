# LIC EXPERIMENT-3
linear integrated circuits
# Aim:
Design and analyze the differential amplifier for the following steps VDD=3.3v, P<=3mw, Vicm =1.65v,Vocm=1.7v,Vp=0.5v perform DC analysis,transient analysis,frequency response and extract the parameters.

Differential Amplifier:

Differential amplifiers consist of two transistors M1 and M2, whose sources are joined together. If the two transistors are connected to different voltage inputs, then the current across M1 and M2 are different due to the gate voltage.
If the voltage supply at the gate terminal is the same, then the current through M1 and M2 is also the same. This configuration is called "Common-Mode Input Voltage Differential Amplifier".
Whatever may be the load resistor, the MOSFET M1 and M2 should not enter the Triode region. It should be verified that the MOSFETs remain in the Saturation Region for proper operation.
![image](https://github.com/user-attachments/assets/3c5dd8db-5be5-4177-aeb6-1e8dcb67f5c0)

Procedure : Make the circuit connection as given above. connect the resister at the source terminal of both mosfet now calculate the value of Iss as power and vdd is given and calculate the Id1 and Id2 now calculate the Rss and Rd

To find the all the values of resistor and current value. we need solve the given queston specification.
P=3mA

Iss=P/VDD=3*10^3/3.3=0.909mA

Is1=Is2=Iss/2=0.4545mA

RD=VDD-Vocm/Iss=3.3-1.7/0.45*10^3=3.55kΩ

Rss=Vp/Iss=0.5/0.909*10^3=0.555kΩ

Finially by solving we get

Iss=0.909mA

I1=I2=0.4545mA

RD=3.55kΩ

Rss=0.555kΩ


# Circuit-1
Components Required: MOSFET(M1,M2 and M3), Resistor,voltage supply's

![Screenshot 2025-03-02 211850](https://github.com/user-attachments/assets/93da95c8-e713-41e4-9a84-5bfd8340b150)

Procedure : Make the circuit connection as given above. connect the resister at the source terminal of both mosfet now calculate the value of Iss as power and vdd is given and calculate the Id1 and Id2 now calculate the Rss and Rd

Now to get the desired values of output voltage and current we have to vary the width and length of both the mosfet we got Length=180nm and width=1.810um

![image](https://github.com/user-attachments/assets/b98dddcc-52cd-4399-b805-8cfdf09220ef)

# DC analysis:
To perform the DC analysis we have to select the {DC op pnt} in the edit simulation command and run the simulation the figure below is the values obtained from the DC analysis
 ![WhatsApp Image 2025-03-02 at 22 53 12_a46b203d](https://github.com/user-attachments/assets/5d1b64f7-54f0-4fa9-becd-fb0ad1096ef7)

Here in dc analysis we got the vout as expected and id1 and id2 we got the same

# Transient analysis:
To perform transient analysis we have to select the transient analysis in the edit simulation and give the stop time as 5ms and run the simulation . and the graph velow shows the transient response of the design.
![image](https://github.com/user-attachments/assets/812e105b-93b8-472e-a969-91521b262dce)

voltage gain 
AV=voutp-p/vinp-p

AV=(1.768-1.632)/(1.697-1.601)

AV=1.424

# AC analysis:
TO perform AC analysis we have to select the ac analysis in the edit simulation command given the values as shown below
![image](https://github.com/user-attachments/assets/fb7e4769-8db7-43af-90e3-606e414762d3)

Gain in db= 20log(AV)

  =20log(1.424)
 
  =3.0707

  # Circuit-2:
  Now replace the R3 resister with a current source : connect a current souce of 0.9mA

  ![image](https://github.com/user-attachments/assets/18c83d5c-c212-40dd-8712-d38a2233c248)

# DC analysis:
To perform the DC analysis we have to select the {DC op pnt} in the edit simulation command and run the simulation the figure below is the values obtained from the DC analysis

![Screenshot 2025-03-02 200403 1](https://github.com/user-attachments/assets/ac6461fc-a913-48e3-b143-1241396432b2)

 # Trasient analysis:

 To perform transient analysis we have to select the transient analysis in the edit simulation and give the stop time as 5ms and run the simulation . and the graph b
 elow shows the transient response of the design

we have to give deg of 180deg to one mosfet and 0deg to the other mosfet and ac amplitude 1 for one mosfet and 0 for other mosfet

![WhatsApp Image 2025-03-02 at 23 23 17_f0153464](https://github.com/user-attachments/assets/f1ceccdc-96f4-4ed8-b5c8-383dcdcd5fbc)

voltage gain 
AV=voutp-p/vinp-p

AV=(1.83-1.5702)/(1.7-1.6)

AV=2.598

# AC analysis:
![WhatsApp Image 2025-03-02 at 23 23 18_44d7f151](https://github.com/user-attachments/assets/c788f6a1-c45c-472d-8566-5e8ff4e75518)

Gain in db= 20log(AV)

  =20log(2.598)

  =8.292

  # Circuit-3:
Now replace the R3 resister with a Mosfet : Given vp=0.4v and wkt vt=0.36v we got the gate voltage of the new mosfet as 0.866v

![image](https://github.com/user-attachments/assets/7dca4dc5-eefa-4e28-a761-768a5f4dabf8)

To get the output voltage and vp and current desired value we have to vary the width and length of the  mosfets

![image](https://github.com/user-attachments/assets/40e17f48-948d-4503-9d80-054e436129e6)![Screenshot 2025-03-02 235357](https://github.com/user-attachments/assets/028f12f7-7a55-4e24-b78d-42b621586501)

# DC analysis:
![image](https://github.com/user-attachments/assets/32cfbdb2-ff0c-4c97-a665-6730f90cce52)

# Transient analysis:
give ac amplitude as 1 for one mosfet and 0 for other mosfet
![image](https://github.com/user-attachments/assets/9469d8ce-e3e1-4541-af3a-cf5e3e77c5f3)

# AC analysis: 

![image](https://github.com/user-attachments/assets/4e00a952-9c8d-4cba-bcf4-9555b8251295)


# INFERENCE:
In this experiment, we seen the working principles of a differential amplifier and its types and configuration.

There are three types of configurations were implemented: resistor , current source , and an NMOS . All the implements work on different ways that results into the cahnge in Voltage gain and stabillity of a mosfet.

when resistor is connected it provides low CMRR,deduce gain voltage,but high bandwidth and also provide negative feedback

But in the case of current source connection it is reciprocal of resistor connection because it has high gain volatge, high CMRR,but slight reduce in the bandwidth compared to the resistor connection.

Highest gain volltage is drewn by the circuit of CMOSN connection

By this we can say at what time/situation is required we can use that configuration.

1.Need more Band width-Use Resistor configuration

2.Need more Gain-Use CMOSN Configuration

3.Need precise CMRR-Use current or CMOSN configuration













  













