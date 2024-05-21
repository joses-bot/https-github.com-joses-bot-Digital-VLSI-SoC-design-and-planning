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

#### Switching threshold  vth = 0.98v  vth = 1.2v  (vgs=Vds)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/437f1e8e-04b9-4d40-a9c5-6b0fd407f5e5)

#### Calculation of rise/fall time  SPICE transient analysis

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/d73c2d43-2e30-48e8-87b1-dea15845865a)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/a38b0625-f3c3-46e5-8d02-84ea076ef21f)

#### Case W/L = 1 In the middle point 1.25v 148ps (rise time)  71ps (fall time)  vm = 0.99

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/dd97e46b-1da0-4e46-a664-dc74dbad56f3)

#### Case W/L = 3 In the middle point 1.25v 64ps (rise time) 2.5ps (fall time)  vm = 1.2

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/a5649d12-c083-4ed9-991c-d2c5f1e1d26f)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/23aa5980-5fda-476c-ae6a-c539e07eef27)



#### Downloading the inverter from github  https://github.com/nickson-jose/vsdstdcelldesign (showing magic tech file)
magic -T sky130A.tech sky130_inv.mag &

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/a754a6c1-b3ec-48b8-96f9-52db2247a387)

#### Selecting layers

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/5d9cb0f1-3c2d-4efb-858c-c88517ffb9ea)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/6c4909b9-c967-40eb-91cb-5cbe3bc253b8)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/00b65ed3-5079-4e6e-8813-4b5028f5658b)

#### CMOS Fabrication Process (16-Mask CMOS Process):

1. Selecting substrat

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/f1b47a19-22f9-4ed4-a1ce-0b957ad26c55)

2. Use photolotography procesure to get the pattern required (adding  mask to protect regions after exposing to UV and then remove it)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/0a7cfee9-5c85-4172-b8b7-87ef663a0efe)

etched the regions to form the patterns then remove the photoresistance layer itself and hen grow the oxide on the required portions (after putting it into a furnace) 
and after further oxide grows creating the isolation areas to protect adjacent transistors

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/50ee5aa6-c93e-4f5d-b40f-16368f2276c0)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/6d9c4265-42ac-4db1-9353-40c2b93860cd)

3. Then create the nwell (p,mos) and pwell (nmos) regions

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/13e1e45d-b22a-4f0d-80a3-72b6453b8b4a)

Then creating one by one each of the nwell and pwell areas using the same photolitography procedure
For the pwell boron is used as ion implanatation to grow the pwell area using high energie

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/6614c3d7-5c7b-40b2-b172-6a181f41228d)

Same procedure to create the nwell using phosphorous ion implantation at a higher energie

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/48a4f733-6d13-4cb8-b48e-c6c1992c4086)

Then put into the furnace to difusse the wells and be ready to create the transistors

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/3df72922-d6a7-43a0-8573-a01f6750b8a2)

4. Create the gate for both p and n transistors (gate determines the threshold voltage by controlling the doping concentration and oxide capacitance) and the nrepaired the quality of oxide
   appyling a polysilicon mask 

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/ea324eef-808a-49f0-95cc-44f51872e320)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/c2a2f89d-287a-45a7-b427-ef227f8a0674)

Magic showing gate mask to form gates

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/9924a83e-0b58-4555-9aee-fdf1efa790e7)

5. Lightly dropped gate formation (attain the dopping profile). Two physical processes to take into account (Hot Electron Effect, Short channel effect)
generates the p-, n- for transsitor drain on pand nwell regions created
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/9c8dc3a0-a538-436b-a5ab-2c7cb711e0ac)

6. Source and drain formation. Using high temperature annealing. Forming p+, n+ and transition layers close to the gate   
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/1d6f8312-bf60-454a-91fc-bc78f8e31d16)

8. From contacts and interconnect (Titanium deposit an etched with RC cleaning)
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/8a988b38-c099-48f7-8f99-9ba790e803fe)

9. Hihger level metal formation (Form a second and third layer of metal interconnect using Tungsten and aluminium layers and photolitograpgry process)
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/28f610c7-1ef5-4cb5-9932-c671c6fa49a7)

#### Introduction to Sky130 basic layers layout and LEF using inverter

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/3d2c85c8-1b0c-4bfc-b28b-a52584506bdf)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/ab6c1b44-b75c-4093-8977-e3ff6d9d854a)

Extract spice netlist from layout

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/5251f4ff-20fe-45aa-8cd2-246a05abe692)

SPICE file is created  sky130_inv.spice

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/b9854760-4292-431b-a85f-cf4f2391d1d5)

Modifying spice model of inverter
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/b9304678-38e5-464d-ad98-256f53baeca8)















   














































