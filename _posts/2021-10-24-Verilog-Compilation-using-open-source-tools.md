---
published: true
---
#### Verilog Compilation using open source tools | iverilog | gtkwave | yosys
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
