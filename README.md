## Ex No: 06 Design-Implementation-of-2-Bit-Multiplier-using-Cadence-Tools 

### Aim:
To design and implement a 2-bit multiplier circuit using Cadence EDA tools, simulate its functionality, and to understand its application in digital arithmetic operations.

### Tools Required:
- Personal Computer
- Cadence Virtuoso Software
  
### Circuit Diagram:

![WhatsApp Image 2024-11-13 at 16 25 39_c1439924](https://github.com/user-attachments/assets/d9cd3034-570c-4b86-8847-b608ccb1c2b5)

### SCHEMATIC SIMULATION:
PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence:

1. Right-click and open the terminal window.
2. Type the following commands and press enter:
   
   • csh&emsp;• source /cadence/install/cshrc&emsp;• virtuoso


#### Procedure for Schematic simulation using Cadence
1.	Now two windows must open
    i) virtuoso/command interpreter window
  	ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window (CIW) for further processing.
   -	Create a New Library
   - Create Schematic Cell view.
   - Create the Symbol for schematic Cell view.
   - Create the test Cell view.
   - Analog simulation by spectre

### Steps for Schematic Simulation using Cadence:
#### i)	Procedure for Creating New Library.
-	File –New – Library
-	Name: Give name for ur library Ex: VLSILAB_EXP_1
-	Enable Attach to an existing technology library, Click OK
-	Attach the library to the technology library gpdk045.Click OK

### ii)	Create Schematic Cell view.
-	Go to 1st window i.e virtuoso (CIW)
-	File-New-Cell view
-	Setup the new file form
    + Library: Select the one you created.
    + Cell: Give the experiment name Ex: Inverter ViewSchematic
    + Type: Schematic press OK
-	Add the required components from the libraries and make the connections.
    + Go to instance fixed menu or use shortcut key “I” from keypad to go instances
    + Click on browse. This opens the library browser
    +	Now select the appropriate library for components like 
    +	Gpdk45 ------------------------nmos1v, pmos1v
    +	Create Input and Output pins
    +	Make the connections by using fixed narrow wire key
    +	Click Check and Save button



![Screenshot 2024-11-13 010613](https://github.com/user-attachments/assets/18e49cb8-64e8-463e-aa1c-4d0d539c8ce1)


 
### iii)	Creating the Symbol for schematic Cell view

-	In the schematic window, execute 
    +	Create – Cell view – From Cell view
    +	The cell view from cell view window appears
    +	Check Lib Name, Cell Name, From View name must be schematic Press ok
-	Now Symbol generation form appears. Click Ok If No changes required
-	A new window with with default symbol is created.
- Edit the symbol if you want to give actual symbol shape else continue.
- Execute Create-Cell view-from cell view
- Library Name and Cell Name must be same which you have used for schematic. Press OK
- Check for the position of pin side.Prss OK
- Edit for the shape by Create-Shape-Choose required options to edit.

![Screenshot 2024-11-13 011204](https://github.com/user-attachments/assets/8d9eb4d3-6f0d-455b-9376-61f9c50a8002)


### iv)	Creating the new test cell view

-	Go to CIW window, Execute File-New-Cell view
    +	Setup the new file form
    +	Library: Select the one you created.
    +	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
    +	View: Schematic
    +	Type: Schematic press OK
-	Follow the step 3(ii) d to make the required connections


![Screenshot 2024-11-13 012223](https://github.com/user-attachments/assets/492bca4f-24bd-4313-81c6-a17e4a089bc9)


 
### Analog simulation by SPECTRE.
-	In test cell view window
-	Launch – ADE L(Analog Design Environment)
    +	Execute Setup—Simulation/directory/Host A new window opens
    +	Set the simulation window to spectre and click ok
    +	Execute Analysis – Choose. A window opens.
    +	Select the type and set the specifications and press OK
    +	Execute Output s—to be plotted – Select on Schematic
    +	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
-	Execute Simulation -- Net list and Run

![Screenshot 2024-11-13 012736](https://github.com/user-attachments/assets/114b52e8-1662-4552-ab3a-2ce99d00933a)



##  For Transient Analysis:
  - In the simulation setup, choose transient analysis.
  - Specify the time range for the analysis (start and stop time).
  - Run the simulation and observe the output waveforms
  

![Screenshot 2024-11-13 012405](https://github.com/user-attachments/assets/8c278590-6e70-4174-906e-1e2ffa44b0ec)

![Screenshot 2024-11-13 223223](https://github.com/user-attachments/assets/74126a6e-af05-4814-9cbf-5a74aa3bf91e)


## Results:
The design and implementation of the 2-bit multiplier using Cadence EDA tools were successfully carried out. The simulation results confirmed the correct operation of the multiplier for all input combinations. 
