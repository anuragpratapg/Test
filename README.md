# Test

# 28T Conventional CMOS Full Adder design
   This repository presents the detailed documentation on designing of Conventional CMOS Full Adder on 28nm CMOS Technology by using Synopsis Custom Compiler.
# Table of Contents
     - Abstract
     - Introduction
     - Reference Circuit
     - Reference Waveform
     - Tools used
     - Schematic in Synopsys Custom Compiler
             - Carry Block
             - Sum Block
             - Top level Full adder 
             - Input pulses for Inputs A,B and C
      - Output Waveform
      - Netlist
      - Calculation of Propagation delay
      - Conclusions
      - Author
      - Acknowledgement
      - References
  
 #  Abstract
    This paper represents 28T conventional full adder design using standard CMOS design. This design is
    implemented on technology 28nm using Synopsys tool. The analysis is carried out using several parameters 
    like power consumption, delay and power delay product on various supply voltages. Full adders are the important 
    components in application such as Digital signal processor, microcontroller, processor and data processing units.
    Keywords— Full Adder, Technology, CMOS, Synopsys

 #  Introduction
    Designing of low-power and high speed Very Large-Scale Integration (VLSI) systems has pop up as highly demands in market 
    due to fast-paced growing technologies in telecommunication and other power applications. Binary addition is the basic 
    components found in most arithmetic and logic components. Hence the realization of Half adder and Full adder nowadays is 
    essential in terms of delay and power consumption. Full adder is designed for addition of two bits (A and B) with input carry C
    in such a way that can take eight inputs together from ‘000’ to ‘111’ and produces two one-bit output i.e. sum and carry out.
    
    Equations of full adder based on the truth table-
    SUM = A  (B  C) 
    COUT = AB + BC + AC OR 
    COUT = C (A ⊕ B) + AB
    
    ![image]{https://user-images.githubusercontent.com/18648566/155855026-08b52406-acd0-4aa8-8270-00cd5e3a2f09.png}
    
    ![image](https://user-images.githubusercontent.com/18648566/155885321-5973448a-3382-4812-be33-be44ddfc9b64.png)
    
                                Fig1: Block Diagram and Truth Table of Full Adder
    The advantages of complementary CMOS logic circuit based full adder design are its layout regularity and stability at low 
    voltage due to the complementary transistor pairs.
    
    A full adder is a digital circuit that performs addition. Full adders are implemented with logic gates in hardware. A full
    adder adds three one-bit binary numbers, two operands and a carry bit. The adder outputs two numbers, a sum and a carry bit. 
    The term is contrasted with a half adder, which adds two binary digits.
    A full adder takes two binary numbers plus a carry or overflow bit. The output is a sum and another carry bit. Full adders 
    are made from XOR, AND and OR gates in hardware. Full adders are commonly connected to each other to add bits to an arbitrary
    length of bits, such as 32 or 64 bits. A full adder is effectively two half adders, an XOR and an AND gate, connected by OR gate.
    
 #  Reference Circuit
    The Fig2 shows the schematic of 28T conventional CMOS design Full Adder. This design is based on complementary pull up and pull
    down topologies and having high noise margin and reliability. The CMOS full adder suffers from large power consumption and high 
    delay. We will also calculate average power consumption by the above circuit.
    
 #  Reference Waveform
    This section presents simulation of reference waveform as shown in below Fig3. Conventional CMOS full adder considered in this work
    are simulated for getting proper outputs along with estimation of propagation delay and average power consumption.
    
 #  Tools used
    - Synopsys Custom Compiler: 
      The Synopsys Custom Compiler design environment includes features for mixed-signal design entry, design debug, 
    simulation management, analysis, and reporting. The Synopsys Custom Compiler™ design environment is a modern solution for
    full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom 
    Compiler provides design entry, simulation management and analysis, and custom layout editing features. It delivers industry-leading
    productivity, performance, and ease-of-use while remaining easy to adopt for users of legacy tools.
    
    - Synopsys Primewave:
      PrimeWave Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF,
      mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. It delivers a seamless simulation
      experience around all the engines of Synopsys PrimeSim Continuum, with comprehensive analysis, improved productivity, and ease of
      use. PrimeWave Design Environment also offers powerful Tcl-based scripting capability enabling easy regressions across thousands of 
      corners.
      
    - Synopsys 28nm PDK kit:
       The Synopsys 28nm process design kit was used in creation and simulation of below design circuit.
       
 #  Schematic in Synopsys Custom Compiler
 #  Carry Block
    - Schematic of Carry block:
      ![Carry_ou_schematic](https://user-images.githubusercontent.com/18648566/155884054-2bce5fd1-5294-4536-83f9-124406af6680.PNG)

    - Symbol of Carry block:
      ![carry_out_schematic](https://user-images.githubusercontent.com/18648566/155884096-c8727081-edfe-40d8-a7c7-2f7ccea1f2a5.PNG)

 #  Sum Block
    - Schematic of Sum Block:
      ![sum_schematic](https://user-images.githubusercontent.com/18648566/155884120-d404c334-2991-4273-a4e9-c17368ca0fe2.PNG)

    - Symbol of Sum Block:
      ![sum_symbol](https://user-images.githubusercontent.com/18648566/155884139-3965aa1a-16a6-4a58-8cc1-8c14509f26a9.PNG)

 #  Top level Full adder 
    - Schematic of Full adder:
      ![top_level_real](https://user-images.githubusercontent.com/18648566/155884230-3cd2f2be-1c51-4395-8989-63cd8c619917.PNG)

    - Symbol of Full adder:
      ![full_adder_symbol](https://user-images.githubusercontent.com/18648566/155884166-36db43f9-6d47-466a-b49d-cbb56788a8a6.PNG)
   
    - Schematic for simulation of Full adder design
      ![top_level](https://user-images.githubusercontent.com/18648566/155884207-44e318bc-4dd6-43e3-a3c2-e675b66c9436.PNG)

 #  Input voltage pulses for Inputs A,B and C
    - Input A:
    ![inputA](https://user-images.githubusercontent.com/18648566/155884249-cd108d1e-5dcc-4180-b745-8b63d2ad9624.PNG)

    - Input B:
    ![inputB](https://user-images.githubusercontent.com/18648566/155884261-4700641b-a300-4e4c-b66e-bc80dd9a227d.PNG)

    - Input C:
     ![inputC](https://user-images.githubusercontent.com/18648566/155884273-b0c499f3-1d0d-49a7-b9e3-1b8cefe0722d.PNG)

 #  Output Waveform
 
    ![output_wf](https://user-images.githubusercontent.com/18648566/155884437-c63cddd7-1125-436b-ba1c-85f729c69b77.PNG)

 #  Netlist
    *  Generated for: PrimeSim
*  Design library name: FULL_ADDER
*  Design cell name: sim_fulladder
*  Design view name: schematic


*Custom Compiler Version S-2021.09
*Sun Feb 27 12:14:17 2022

.global gnd!
********************************************************************************
* Library          : FULL_ADDER
* Cell             : carry_out
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt carry_out a b c cout coutb gnd_1 vdd
xm51 cout coutb gnd_1 gnd_1 n105 w=0.1u l=0.03u nf=1 m=1
xm43 net2 a gnd_1 gnd_1 n105 w=0.4u l=0.03u nf=1 m=1
xm42 coutb b net2 gnd_1 n105 w=0.4u l=0.03u nf=1 m=1
xm41 net3 b gnd_1 gnd_1 n105 w=0.4u l=0.03u nf=1 m=1
xm40 net3 a gnd_1 gnd_1 n105 w=0.4u l=0.03u nf=1 m=1
xm39 coutb c net3 gnd_1 n105 w=0.4u l=0.03u nf=1 m=1
xm64 cout coutb vdd vdd p105 w=0.2u l=0.03u nf=1 m=1
xm56 net1 a vdd vdd p105 w=0.8u l=0.03u nf=1 m=1
xm55 coutb b net1 vdd p105 w=0.8u l=0.03u nf=1 m=1
xm54 net4 b vdd vdd p105 w=0.8u l=0.03u nf=1 m=1
xm53 net4 a vdd vdd p105 w=0.8u l=0.03u nf=1 m=1
xm52 coutb c net4 vdd p105 w=0.8u l=0.03u nf=1 m=1
.ends carry_out

********************************************************************************
* Library          : FULL_ADDER
* Cell             : sum
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt sum a b c coutb gnd_1 sum vdd
xm66 sum net4 gnd_1 gnd_1 n105 w=0.1u l=0.03u nf=1 m=1
xm50 net8 a gnd_1 gnd_1 n105 w=0.3u l=0.03u nf=1 m=1
xm49 net7 b net8 gnd_1 n105 w=0.3u l=0.03u nf=1 m=1
xm48 net4 c net7 gnd_1 n105 w=0.3u l=0.03u nf=1 m=1
xm47 net4 coutb net9 gnd_1 n105 w=0.2u l=0.03u nf=1 m=1
xm46 net9 c gnd_1 gnd_1 n105 w=0.2u l=0.03u nf=1 m=1
xm45 net9 b gnd_1 gnd_1 n105 w=0.2u l=0.03u nf=1 m=1
xm44 net9 a gnd_1 gnd_1 n105 w=0.2u l=0.03u nf=1 m=1
xm65 sum net4 vdd vdd p105 w=0.2u l=0.03u nf=1 m=1
xm63 net5 a vdd vdd p105 w=0.6u l=0.03u nf=1 m=1
xm62 net6 b net5 vdd p105 w=0.6u l=0.03u nf=1 m=1
xm61 net4 c net6 vdd p105 w=0.6u l=0.03u nf=1 m=1
xm60 net10 c vdd vdd p105 w=0.4u l=0.03u nf=1 m=1
xm59 net10 a vdd vdd p105 w=0.4u l=0.03u nf=1 m=1
xm58 net10 b vdd vdd p105 w=0.4u l=0.03u nf=1 m=1
xm57 net4 coutb net10 vdd p105 w=0.4u l=0.03u nf=1 m=1
c3 sum gnd_1 c=2p
.ends sum

********************************************************************************
* Library          : FULL_ADDER
* Cell             : full_adder
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
.subckt full_adder a b c cout gnd_1 sum vdd
xi0 a b c cout net16 gnd_1 vdd carry_out
xi1 a b c net16 gnd_1 sum vdd sum
.ends full_adder

********************************************************************************
* Library          : FULL_ADDER
* Cell             : sim_fulladder
* View             : schematic
* View Search List : hspice hspiceD schematic spice veriloga
* View Stop List   : hspice hspiceD
********************************************************************************
xi0 a b c cout gnd_1 sum vdd full_adder
v40 gnd_1 gnd! dc=0
v39 vdd gnd_1 dc=1.8
v43 a gnd_1 dc=0 pulse ( 1.8 0 0 10n 10n 5u 10u )
v42 b gnd_1 dc=0 pulse ( 1.8 0 0 10n 10n 10u 20u )
v41 c gnd_1 dc=0 pulse ( 1.8 0 0 10n 10n 20u 40u )
c2 cout gnd_1 c=2p
c1 sum gnd_1 c=2p

.option primesim_remove_probe_prefix = 0
.probe v(*) i(*) level=1

.temp 25

.option primesim_output=wdf

.option parhier = LOCAL

.end

 #  Calculation of Propagation delay 
 #  Conclusions
    The addition of single bit is achieved using 28T full adder. We get desired output waveform of Sum and Carry by applying appropriate 
    input supply.
    
 #  Author
    Anurag Pratap Singh
    Bangalore- 560100
    
 #  Acknowledgement
    1. Cloud based Analog IC Design Hackathon
    2. IIT, Hyderabad
    3. Synopsys India
    4. VLSI System Design Pvt Ltd, India
    5. Especial Thanks to Kunal Ghosh(Co-founder of VSD pvt ltd), Chinmaya Panda (IIT, Hyderabad), Sameer Durgoji and his colleagues.
    
 #  References
    1. Omid Kavehei, Mostafa Rahimi Azghadi, Keivan Navi and Amir-Pasha Mirbaha, Design of Robust and HighPerformance 1-Bit CMOS Full 
    Adder, IEEE Computer Society Annual Symposium on VLSI.
    2. CH. Haritha, L. Sarika, “Design of CMOS Full Adder Cells for Arithmetic Applications”, International Journal of Engineering
    Research & Technology (IJERT) Vol. 2 Issue 9, September–2013
    3. S. Wairya, Himanshu Pandey, R.K.Nagaria and S. Tiwari, Ultra Low Voltage High Speed 1-Bit CMOS Adder, Member, IEEE.

     
