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






