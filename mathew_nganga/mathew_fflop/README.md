This is a flipflop example, which is a makefile project and so no need for an IDE. 
Just cd into this folder and run the command 

   


A flip flop is a two stable state circuit that can be used to store a state information.<br>
A D flipflop is a type of flip flop that captures the value of <sup>D_input</sup> at a difinite portion of clock cycle<br>
such as the rising edge<br>

That captured value becomes the Q output at other times,the output Q does not change.<br>

Dff therefore is viewed as a memmory cell<br>
<p align="left">
  <img src="truthtable-flop.png" width="100"/>
</p>

###Circuit:
<p align="left">
  <img src="dff_cicuit.png" width="200"/>
</p>

Model of computation:
<p align="left">
  <img src="MOC-FLOP.png" width="400"/>
</p>
Results:
The above MOC was implemented in systemc (code in this folder) and the following output found from traced signals.<br>
Traced signals timing diagram:
<p align="left">
  <img src="timingF_diagram.vcd" width="400"/>
<p>


