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

Showing different layers in magic
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/3d2c85c8-1b0c-4bfc-b28b-a52584506bdf)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/ab6c1b44-b75c-4093-8977-e3ff6d9d854a)

Extract spice netlist from layout

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/5251f4ff-20fe-45aa-8cd2-246a05abe692)

SPICE file is created  sky130_inv.spice

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/b9854760-4292-431b-a85f-cf4f2391d1d5)

Modifying spice model of inverter
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/b9304678-38e5-464d-ad98-256f53baeca8)
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/f564452d-835b-4a0a-adba-2c068a624fa1)

Characterization of cell: Calculation rise time, cell rise delay

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/1a0583d1-9dc6-4ab7-8fc7-cb30935251ef)

rt = 0.0418ns  rdelay = 0.037ns

#### introduction to Magic tool options and DRC rules
Sky130 Gihub repository 
https://github.com/google/skywater-pdk

Get Lab files/unzip files for performing DRC corrections

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/579b6914-155e-4f6c-a991-6450a0ce636d)

vi .magicrc
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/c8c263b0-3c43-4e27-84b5-44412e2303ba)

invoking magic magic -d XR and open file met3.mag (Different layouts with different DRC rules are shown)
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/9821569e-58e7-4b60-bac6-a40e477eacd2)
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/2e9fbb44-2f3c-40db-a976-c3d2cf055e93)

Poly error example

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/2aa9b616-e90e-451c-bb10-d69bef1bf21b)

Fixing rule (addding rules for: spacing npres allpolynonres and spacing xhrpoly,uhrpoly,xpc allpolynonres)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/78ac529c-212a-4a28-986f-af9bf8d7d248)

More examples .....

#### Pre-layout timing analysis and importance of good clock tree
Guidance rules:
When designing standard cells, the Input and output ports must lie on the intersection of the Vertical and Horizontal tracks.
The width of the standard cell must be an odd multiple of the track pitch and the height of the standard cell should be an odd multiple of track vertical pitch.

Layout is already done. Open the track file pdk/sky130/libs.tech /openlane/sky130_fd_sc_hd/track.info. Convert grid info to track info (used on routing)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/b7d9aa48-3e9a-467e-8a05-a7cf3f58265a)
Changing grid following track file
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/96611ea2-c569-4521-9794-ab3f559e2c57)

Renaming file to extract lef file from layout:  lef write (command)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/2676d383-61a3-4a98-9650-fc032b53a410)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/b5966b0a-84f6-4dc6-8b02-286f68777dfe)

#### Dealing with timing libs and include new cell in synthesis modifying config.tcl
Run openlane again with modified config
set ::env(LIB_SYNTH)   "./designs/picorv32a/src/sky130_fd_sc_hd__typical.lib"
set ::env(LIB_FASTEST) "./designs/picorv32a/src/sky130_fd_sc_hd__fast.lib"
set ::env(LIB_SLOWEST) "./designs/picorv32a/src/sky130_fd_sc_hd__slow.lib"
set ::env(LIB_TYPICAL) "./designs/picorv32a/src/sky130_fd_sc_hd__typical.lib"

set ::env(EXTRA_LEFS) [glob $::env(OPENLANE_ROOT)/designs/$::env(DESIGN_NAME)/src/*.lef]

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/7b92537d-3ba4-4a22-9f8f-21f314cb2235)

Invoking run_synthesis again and checking timing violations

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/56d89e19-373c-4290-a5f0-ec27656f9a94)

Timing modelling using delay tables

Modeling using tables the delays depending on the input/ouput capacitance load. Delay tables will becomethe timing models for that particular buffer to the corresponding size

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/e8757ec9-a791-46a7-9977-c363b17d2c3d)

Changing strategy parameters to reduce timing slack

Design seems to meet timing after changes:

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/5141fd6b-766b-4dbe-8d21-8ec755cc38a2)

Area increased a bit but timing is better

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/71a62416-9358-4df6-b03d-04ec4226ab06)

run_floorplan gives an error. basic_macro_placement command is failing since EXTRA_LEFS variable was added in config.tcl and it is assumed as a macro but it is not. The work around is to comment call on basic_macro_placement inside script OpenLane/scripts/tcl_commands/floorplan.tcl (this is okay since we are not adding any macro to the design).

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/79ea5d6b-cfc3-4972-b17c-0d0dd924e3d8)

work around floorplan
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/924a0fd6-2a39-4e04-876e-f12754c1b5a2)

run_placement
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/3f95b1ec-6320-46dd-aa49-9da83be5331f)

New inverter added shows in def file after placement (def file and in magic)
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/ee6f8835-91a7-4a47-b043-82dff044f167)

![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/0a976c09-3b74-4c14-8591-f8a6c59590a8)

#### Timing Analysis STA (Pre-insertion of lock tree STA)

Basic framework consideredb- setup time (including uncertinty) Θ < T - S - SU
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/4778cbae-8ffc-4cb9-9df5-be85b1dce8e8)

#### Open STA commnads:

report_net -connections _18666_
replace_cell _18666_ sky130_fd_sc_hd__buf_4`
report_checks -from _18666_ -to _187775_ -fields {cap slew nets} -digits 4
report_wns
report_tns
report_worst_slack -max

#### SDC File commands:

create_clock clk  -name sys_clk  -period 20
create_clock [get_ports clk]  -name sys_clk  -period 20  (another variant)

I/O Delay
set_input_delay 2 -clock [get_clock clk] [all_input]
set_output_delay 0.45 -clock [get_clock clk] [all_output]

set_max_fanout 13 [current_design]
set_load 10 [all_outputs]

set_clock_transition 0.25 [get_clocks clk]  (rise & fall time)

set_driving_cell -lib_cell sky130_fd_sc_hd__inv_2 -pin Y clk_master   (external driver)
set_driving_cell -lib_cell sky130_fd_sc_hd__inv_4 -pin Y clk          (external driver)

#### Clock Tree Synthesis Process  (run_cts) after succesfully ran run_floorplan, run_placement
Goal is to reduce the clock skew and the clock crosstalk

#### run_cts is located on /OpenLane/scripts/tcl_commands/cts.tcl, and it will OpenROAD and will run TritonCTS. Some parameters can be tweak to help meeting timing
![image](https://github.com/joses-bot/https-github.com-joses-bot-Digital-VLSI-SoC-design-and-planning/assets/83429049/8ad7b0c5-efd9-4b4d-9023-204f351d2e6a)



































































   














































