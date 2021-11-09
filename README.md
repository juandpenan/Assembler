# Assembler

Solution for the [Factory IO](https://factoryio.com/) assembler [scene](https://youtu.be/IC7GJVJ_QlA). Done in [twincat 3](https://www.beckhoff.com/en-en/support/download-finder/software-and-tools/) with structured text.

# Twincat 3 - Factory IO Connection
To connect twincat with factory io the OPC-UA protocol can be used, to set up the connection the function [TF 6100](https://www.beckhoff.com/en-us/products/automation/twincat/tfxxxx-twincat-3-functions/tf6xxx-tc3-connectivity/tf6100.html) must be installed. In addition, the license of this function must be enabled, as well as the TCM file option.

# Working modes
- **Waiting to Start:** The scene will remain inactive until you hit the start button. this working mode is the default when you first run the program.
- **Working:** After you have pressed the start button the scene will work correctly until you hit either stop or emergency buttons.
- **Stopped:** If you hit the stop button, the bases conveyor will wait to finish the ongoing product and stop the whole process. You must press start to come back to the working mode.
- **Emergency** After pressing the emergency button the whole plant will stop immediately and you must remove all bases and lids, release the emergency button and then press start to change to the working mode. 

# I/O Connections 
To connect the variables declared in twincat 3 with the factoryIO sensors and actuators you must follow the next image.
<p align="center">
  <img src="https://github.com/juandpenan/Assembler/blob/main/Screenshots/Inputs-Outputs.PNG?raw=true"/>
</p>





         

