## EXP02--Design-Implementation-of-Full-Custom-2-1-MUX-using-Cadence-EDA-Tools

## Aim:
To design and implement a 2:1 multiplexer (MUX) circuit using Cadence EDA tools, analyse its functionality and performance, and understand the principles of digital logic design, including schematic creation, layout design, and simulation.

## Tools Required:

•	Personal Computer

•	Cadence Virtuoso Software


## Circuit Daigram:

![IMG-20241115-WA0003](https://github.com/user-attachments/assets/36ab9035-708c-4d5b-91be-eb0c35569e7c)


## SCHEMATIC SIMULATION:

PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence
1.	Right Click and open the terminal window
2.	Type the following commands as follows and press enter.
•	csh
•	source /cadence/install/cshrc
•	virtuoso 
Procedure for Schematic simulation using Cadence

1.	Now two windows must open i)virtuoso/command interpreter window ii)”Whats New…”
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window(CIW) for further processing.
i.	Create a New Library
ii.	Create Schematic Cell view.
iii.	Create the Symbol for schematic Cell view.
iv.	Create the test Cell view.
v.	Analog simulation by spectre


i)	Procedure for Creating New Library.
•	File –New – Library
•	Name : Give name for ur library Ex: VLSILAB_EXP_1
•	Enable Attach to an existing technology library, Click OK
•	Attach the library to the technology library gpdk045.Click OK
ii)	Create Schematic Cell view.
•	Go to 1st window i.e virtuoso(CIW)
•	File-New-Cell view
•	Setup the new file form
	  Library: Select the one you a created.
	  Cell : Give the experiment name Ex: Inverter View_Schematic
	  Type: Schematic press OK
•	Add the required components from the libraries and make the connections.
	Go to instance fixed menu or use shortcut key “I” from keypad to go instances
	Click on browse. This opens the library browser
	Now select the appropriate library for components like 
	Gpdk45 ------------------------nmos1v,  pmos1v
	Create Input and Output pins
	Make the connections by using fixed narrow wire key
	Click Check and Save button
![Screenshot 2024-11-16 183728](https://github.com/user-attachments/assets/0c992b99-0f8e-4217-a75c-5f429cbed186)




 iii)	Creating the Symbol for schematic Cell view
•	In the schematic window, execute 
	Create – Cell view – From Cell view
	The cell view from cell view window appears
	Check Lib Name, Cell Name, From View name must be schematic Press ok
•	Now Symbol generation form appears. Click Ok If No changes required
•	A new window with with default symbol is created.
•	Edit the symbol if you want to give actual symbol shape else continue.
•	Execute Create-Cell view-from cell view
•	Library Name and Cell Name must be same which you have used for schematic. Press OK
•	Check for the position of pin side.Prss OK
•	Edit for the shape by Create-Shape-Choose required options to edit.

![Screenshot 2024-11-16 182710](https://github.com/user-attachments/assets/9aa3977a-3267-4846-9856-c60b6ad3ccf2)



iv)	Creating the new test cell view
•	Go to CIW window, Execute File-New-Cell view
	Setup the new file form
	Library: Select the one you created.
	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test
	View: Schematic
	Type: Schematic press OK
•	Follow the step 3(ii) d to make the required connections
![Screenshot 2024-11-16 182426](https://github.com/user-attachments/assets/ba18eb3b-ae4e-416f-bc7e-e5e195df9ec4)


## Analog simulation by SPECTRE.
•	In test cell view window
•	Launch – ADE L(Analog Design Environment)
	Execute Setup—Simulation/directory/Host A new window opens
	Set the simulation window to spectre and click ok
	Execute Analysis – Choose. A window opens.
	Select the type and set the specifications and press OK
	Execute Output s—to be plotted – Select on Schematic
	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
•	Execute Simulation -- Net list and Run
![Screenshot 2024-11-16 183632](https://github.com/user-attachments/assets/8552716f-ffe9-4ab8-826e-60ac42a6256e)


## For Transient Analysis Settings and Output
![Screenshot 2024-11-16 182843](https://github.com/user-attachments/assets/84e44a61-84d2-4533-8bd7-3cc204ee505c)

## Output
![Screenshot 2024-11-16 183407](https://github.com/user-attachments/assets/d5996e14-f8db-41e3-9fde-63509869924f)





 
## Results:
1.	The experiment successfully demonstrated the design and implementation of a 2:1 MUX using Cadence EDA tools. 
2.	The successful verification through schematic, layout, and simulation underscores the effectiveness of using Cadence EDA tools for digital circuit design.
