---
published: true
---
###### Verilog Stratified Event Queue
<iframe width="560" height="315" src="https://www.youtube.com/embed/FExnMzqH_Wk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

-------------------------------------------------------------
###### Verilog Compilation using open source tools | iverilog | gtkwave | yosys
<iframe width="560" height="315" src="https://www.youtube.com/embed/Y3YJvkR-XR4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
In this video we will see how to compile verilog files on linux environment using open source tools.
`iverilog` is used to compile the `.v` file.
`Gtkwave` is used to view the waveform.
`Yosys` is used to view the synthesized version of the design file.
###### commands
 - iverilog -o tb tb.v
 - vvp tb
 - gtkwave test.vcd
 - yosys
 	- yosys> read_verilog ha.v
    - yosys> opt
    - yosys> show

-------------------------------------------------------------------
###### Good Positive edge Detection Circuit Indicating for one clock pulse
<iframe width="560" height="315" src="https://www.youtube.com/embed/DV8X_fsI7mI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
Design a good edge detection circuit. Using two D flip-flop, the output stays high for one clock pulse if the edge is detected, while using only one D flip-flop, we will get a small spike in the output for small duration duration.

---------------------------------------------------------------------
###### Mux as a universal logic. Design AND, OR, NOT, XOR using 2:1 mux
<iframe width="560" height="315" src="https://www.youtube.com/embed/zYY1MTP3NVE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

----------------------------------------------------------------------
###### Digital Design on a piece of paper using vectored mux, adder and comparator (New approach)
<iframe width="560" height="315" src="https://www.youtube.com/embed/g8I3lX3NaJw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
We will be designing three digital circuits on a piece of paper and than coding it in verilog. We will be using only three basic components to design the circuits. Vectored adder, vectored mux and vectored comparator. Using this method it is really easy to visualize the code as well as the design.
 - 4:2 MSB Priority Encoder.
 - Selecting Maximum and Minimum values from two n-bit numbers.
 - Generating next seconds for a watch.
-----------------------------------------------------------------------