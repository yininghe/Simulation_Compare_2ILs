# Simulation_Compare_2ILs
Use simulation to study the double layer structure difference between 2 Ionic Liquids (ILs): [Bmpy][NTf2] vs. [Bmim][NTf2]

The structures of the 2 ILs: 
![IL Structures](images/IL_structure.bmp) 

Ionic liquid (IL) is found as a good type of electrolyte material for fabricating miniaturized and highly sensitive hydrogen sensors. In general, 2 kinds of IL molecules are commonly used: [Bmpy][NTf2] vs. [Bmim][NTf2]. On the one hand, previous experiments show that [Bmim][NTf2] demonstrates higher ionic diffusivity and conductivity than [Bmpy][NTf2] [1,2]. However, recent experiments demonstrated that [Bmpy][NTf2] is more sensitive than [Bmim][NTf2] as an hydrogen sensor. Here we used molecular dynamics (MD) to investigate the structural difference of the 2 ILs, focusing especially on the regions near the electrolyte|electrode interphase, in order to find out what caused the hydrogen sensing difference of the 2 IL electrolytes.

We build a Pt-Electrode|IL-Electrolyte|Pt-Electrode electrochemical sensor, the schematic of our simulated structure can be seen from: Simulation_Compare_2ILs/images/method_cell.bmp.

![Hydrogen Sensor Schematic](images/method_cell.bmp) 

We used the lammps software (version: 22Dec2022) to implement our MD simulations (T = 340K). The whole simulation involve the following 3 sub-steps: 

(1) NPT for only ILs; 

(2) NVE for Pt-electrode + ILs

(3) NVE for hydrogen + ILs + Pt-electrode, this is also the step in which the generated data will be used for data analysis and property calculation.

Here we shared the input data files for each of the 3 steps for both ILs, to maintain the standards of transparency, research reproducibility, and to promote the reuse of new findings.

Reference:

[1] H. Tokuda, et al., doi: 10.1021/jp047480r.

[2] H. Tokuda, et al., doi: 10.1021/jp053396f.

[3] Y. Tang, et al., doi: 10.1021/acs.jpcc.6b07067.

[4] Y. Tang, et al., doi: 10.1039/C8AN00577J.
