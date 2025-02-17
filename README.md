# Tejaswini-M-R-
# Experiment-1
Question:the power given is P=50uW , perform DC analysis , Transient analysis and AC analysis for the given circuit and check what happens when the width is increased or decreased of each mosfet.
# Design-1:
![Screenshot 2025-02-17 213914](https://github.com/user-attachments/assets/3c6bf7a7-66ff-4d83-989d-fcc4213c9ba0)

Aim:To determine the DC operating point, calculate the gain using transient and AC analysis. Components: MOSFET, resistor, DC power supply. Procedure: Connect the circuit as described above. Attach the RD resistor to the drain terminal, the DC power supply to the gate terminal, and the source to ground. Set the input voltage to 0.3V and Vdd to 1.8V. Using the power formula P=VI with power = 50uW and voltage = 1.8V, we can find the current to be 27µA. By adjusting the MOSFET’s width and length, we can achieve the desired drain current Id. Given that the length is 180nm, adjusting the width to 910um will yield the required current.

   1.DC analysis:
     Inorder to simulate the DC analysis we have to select the option called [DC op pnt] in the 
     edit simulation command and run the simulation,we can see the vales obtained from the DC 
     analysis in the figure below
     
![Screenshot 2025-02-17 213709](https://github.com/user-attachments/assets/0f73ed0e-c699-4f84-8e6e-209da04c093c)


   2.Transient Analysis:
     Inorder to simulate the transient analysis we have to select the option called transient 
     analysis in the edit simulation and give the stop time as 5ms and run the simulation,the 
     graph in the below figure shows the transient response of the design.
     ![Screenshot 2025-02-17 214007](https://github.com/user-attachments/assets/41deaa9d-cbbf-44b6-af12-61eec643adc5)


   3.AC analysis:

   
   Inorder to perform the ac analysis we need to select the ac analysis option in the edit.
     simulation command.
     
   we should give the valuess as shown below

     
   ![Screenshot 2025-02-17 214129](https://github.com/user-attachments/assets/26d0a053-9f57-4466-bd28-1cf7da98944f)

     
   the graph shown is the ac analysis

     
   ![Screenshot 2025-02-17 214605](https://github.com/user-attachments/assets/e44973fe-fbf9-4e5a-9ae0-2110d13577b5)


 Result:

   1.DC analysis:

 The calculated drain current aligns with the expected value based on power and voltage, 
     with Id = 27uA. By adjusting the MOSFET's channel dimensions L = 180nm and W = 910um the 
     current requirement was successfully met. The circuit performs as expected under DC 
     conditions.

 2.Transient Analysis:

   The transient response graph shows the circuit's behavior over time. The response is 
     smooth, with no unexpected delays or distortions. The circuit reacts appropriately to 
     changes, indicating that it is stable and functions as expected.

   3.AC Analysis

 The ac response graph confirms us that the circuit will remain stable at different 
     frequencies,the circuit mainitains its performance across the tested frequency range.

 Inference

   The experiment confirms that by selecting the appropriate MOSFET dimensions, the drain 
    current can be effectively controlled.The width of the MOSFET significantly impacts the 
    drain current, indicating that any variation in width directly affects the output current.
    Increasing the width results in a higher Id, while decreasing the width reduces Id.The 
    design aligns with theoretical predictions and matches the practical values observed 
    in the experiment.



# Design-2
   Aim : To find DC operating point find gain using transient analysis and AC analysis.

   Components : Mosfets M1 and M2 DC power supply.

   Procedure :

   Make the circuit connections as show abovce.
   Connect dc power supply to the gate terminal.
   Connect the source terminal to the ground.
   Set the input voltage by obtaining Vtc curve and Vdd to 1.8 V.

   Using the Formula for Power

   P=vi

   We will get the Values of Id

   Id= 27uA


   we have to get the output current Id for the given circuits by adjusting the values of L & W of both the MOSFETS

   
   by adjusting the value of width and length of the mosfet we will get the current Id 
   As length is given 180nm by adjusting we will get width=0.61um this value of width and length is for both the mosfet

 1.DC Analysis:

   
   To perform the DC analysis we have to select the {DC op pnt} in the edit simulation command and run the simulation
     the figure below is the values obtained from the DC analysis


 
   2. Transient Analysis

   
   To perform transient analysis we have to select the transient analysis in the edit simulation
   and give the stop time as 5ms and run the simulation .
   and the graph velow shows the transient response of the design.



   3. AC analysis
 

   TO perform AC analysis we have to select the ac analysis in the edit simulation command given the values as shown below



   the Graph shown is the ac analysis


   
   RESULTS:

  1.DC analysis
  
  
  The calculated drain current Id aligns with the expected value based on power and voltage  where the value of Id = 27um 
  By fine-tuning the channel dimensions  of both MOSFETs  the desired current was achieved L=180nm and W=0.61um for both mosfets
  The circuit operates correctly within the selected DC parameters 

  
  2.Transient Analysis:

  The transient response graph confirms that the circuit transitions smoothly over time.
  The circuit responds effectively to input variations, indicating stable operation.

  
  3.AC Analysis:

  The AC response graph confirms that the circuit maintains stability over the tested frequency range.
  The circuit functions as expected under AC conditions.


  INFERENCE:


 the experiment validates that by choosing the correct mosfet dimensiions the drain current can be effectively regulated.

The voltage transfer characteristics  helped to select the correct operating voltage  for saturation.

 M1  has a stronger influence on ID, meaning its width significantly affects the output current  Increase in width increases Id  and vice-versa.
 M2 has a smaller influence on ID  meaning changes in its width result in only minor changes  in Id. Increase in width increases ID by small value and vice-versa.

    


   

     


