### Digital-VLSI_SoC-VSD
#### Running Openlane

![image](https://github.com/joses-bot/jose_vdiasat_workshop/assets/83429049/b6fb7ec7-8a1f-4fa8-a01a-fdc7d7176bda)

#### Issuing package command

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/d9057f8a-8e40-4e00-aeb1-0f19f5176c26)

#### Preparing the design to use picorv32a

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/0241eea7-cef5-421a-8719-85e4187031b7)

#### Files Generated

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/48b63560-92b0-4168-969a-76a9e9b88a5a)

#### Issuing command run_synthesis 

#### OpenLane invokes the following

    - Yosys - RTL Synthesis and maps to yosys generic cells
    - abc - Technology mapping with the Skywater130 PDK
    - OpenSTA - This does the Static Timing Analysis on the netlist generated after synthesis
    
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/c8cdfd5a-183f-41d2-a5e1-eb9dc007d620)

#### View Synthesis statistics
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/54ba3345-8de9-43c6-9d06-b9ce96074a6b)

#### Report Folder created

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/48a9ad00-c149-411e-a26a-0676b82f71fc)

#### The openSTA tool generated the timing reports.

    - total negative slack = -759.46
    - worst negative slack = -24.89

#### Utilisation Factor  [From the synthesis statistics]

    The flop ratio is defined as the ratio of the number of flops to the total number of cells
    Here flop ratio is 1613/14876 = 0.1084 (10.8%) 

#### Chip area module 147712.918400

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/8a8edff8-4f4e-4717-8699-b56f78d1d177)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/b4bb13fd-ccd5-4e3f-a582-1317eb7d9ba6)

#### picorv32a  config.tcl

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/e550c7cc-490e-4f19-81d6-37925d6b8981)

#### Issuing command %run_floorplan

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/e9b3ca30-0170-4640-8c21-cf04129ba8ca)

#### Inserting cells

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/2d2f706f-cce1-4ff7-ba5a-130caa28e2f9)

#### results after floorplan picorv32a.floorplan.def generated

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/11d88816-87b9-4cb7-8ea5-c79a94aebca5)

#### Layout using MAGIC

#### Invoking magic: 
####  magic -T /home/vsduser/Desktop/work/tools/openlane_working_dir/pdks/sky130A/libs.tech/magic/sky130A.tech lef read ../../tmp/merged.lef def read picorv32a.floorplan.def &

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/95f7fd0b-3edd-4b80-80a1-d5a7cc38f0a4)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/f8fa8ca6-d75c-48d4-a359-82a268d77ab7)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/a3106ddd-0df0-40b7-a3c0-56676752afd0)

#### Placement  %run_placement

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/83377c29-65b3-4aa4-9adf-3e37441acebb)


![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/c6325c94-f56f-4b69-a1c9-9e8102233804)

#### Reading Placement.def into magic

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/cfee7fba-d4a9-49f4-bb6d-bb2ee42b4bcd)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/203bbc7a-6607-417a-94b6-72c2aab9b7e6)

#### Zoom on magic view showing placement of standard cells

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/0bbb6bb0-bff5-4025-98ba-1bceaaa2fba4)

#### Design library cell using Magic Layout and ngspice characterization
#### BASIC CMOS PN INVERTER

Component connectivity
Component values
Identify modes

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/5af31a19-806a-471f-ae04-603790165a11)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/e0ecda95-8900-4ab1-8754-a19b2c051d8d)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/7e85f712-27e6-4a33-a2a8-9599ecac5dc0)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/28e407a6-dcd1-41b8-99b7-f1e89f7cbbee)

#### SPICE commands:

source [filename].cir
run
setplot 
dc1 
plot out vs in 

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/a0a055be-7891-427e-9f2b-4bc1ef7f3da8)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/897e7638-d6e0-4a27-94fd-8bc7eda38dd5)

#### Changing the pmos W=0.9375u

#### Switching threshold  vth = 0.98v  vth = 1.2v

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/437f1e8e-04b9-4d40-a9c5-6b0fd407f5e5)


#### Downloading the inverter from github  https://github.com/nickson-jose/vsdstdcelldesign (showing magic tech file)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/a754a6c1-b3ec-48b8-96f9-52db2247a387)

#### Selecting layers

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/5d9cb0f1-3c2d-4efb-858c-c88517ffb9ea)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/6c4909b9-c967-40eb-91cb-5cbe3bc253b8)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/00b65ed3-5079-4e6e-8813-4b5028f5658b)



























