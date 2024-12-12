<h1>Digital VLSI SoC Design and Planning</h1>


<h2>Inception of open-source EDA, OpenLANE and Sky130 PDK</h2>
<details>
<summary> Day-1  </summary>
<p>

Open Source ASIC Flow

![image](https://github.com/user-attachments/assets/43cd04c9-bacb-4a7b-9661-b91db6d0f76c)
 
OPENLANE ASIC Design Flow

![image](https://github.com/user-attachments/assets/55e324b9-1826-4958-8b8c-d9a8e1f8893f)

Library Characterisation and Modeling

![image](https://github.com/user-attachments/assets/c3f7fbb2-0e17-4660-9e04-65fdc821e6d3)

Cell Design Flow (Input Stage)

![image](https://github.com/user-attachments/assets/f92e4996-720b-4c4d-9c53-2a7fa258cdd7)

Cell Design Flow (Layout Design)

![image](https://github.com/user-attachments/assets/113edc69-7d9d-4e95-92e9-60ed8365c029)

Cell Design Flow(Characterization)

![image](https://github.com/user-attachments/assets/6840352f-244c-4991-a639-cca24e28cfc0)

Timing Characterisation

![image](https://github.com/user-attachments/assets/44ddca7b-d27f-4348-b6f4-cc3d0d4d0039)

Propogation Delay Graph vizualization

![image](https://github.com/user-attachments/assets/2e73f5ca-a910-4dfe-85e1-77177fbbf116)

### Labs Screenshots

1.Openlane start command

![image](https://github.com/user-attachments/assets/ea0aa657-230b-4222-a112-81f23bed24a4)

2.Run Synthesis command

![image](https://github.com/user-attachments/assets/3f20b98f-d4b2-4c84-8f47-fdaca0a8f58f)
 </p>
</details>
<h2>Good floorplan vs bad floorplan and introduction to library cells</h2>
<details>
<summary> Day-2 </summary>
<p>

1.Run Floorplan command 

![image](https://github.com/user-attachments/assets/f4a4df09-73ba-458a-a05a-16a4f36a7e88)


2.Command running Floorplan in Magic

![image](https://github.com/user-attachments/assets/03c816d3-b82d-41b4-bc21-6a930de2a0c7)


3.Command running Placement

![image](https://github.com/user-attachments/assets/293b0831-1137-43fa-b41f-07dc6153377f)
![image](https://github.com/user-attachments/assets/e126cddd-b7ff-4e38-af02-fc2cc496da39)


4.Screenshot of def file of placement in magic 

![image](https://github.com/user-attachments/assets/57598941-1de5-4695-a57e-f84325b9bc14)




 
</p>
</details>

<h2>Design library cell using Magic Layout and ngspice characterization</h2>
<details>
<summary>Day 3  </summary>
<p>
<p>1.Git cloning custom inverter standard cell design from github repository of Nickson Jose sir</p> 


<p>2. Viewing inverter in magic and also the console for other interactions </p>
3. 
![WhatsApp Image 2024-12-11 at 19 45 38_7f753439](https://github.com/user-attachments/assets/ccd0b068-34d0-4839-a0ad-c52d0a6de4ca)


3.Identified PMOS from the layout using "s" key

![WhatsApp Image 2024-12-11 at 19 48 22_eb5d4d74](https://github.com/user-attachments/assets/40c40d63-3329-41a6-9ada-0162fde429ad)


4.Identified NMOS from the layout using "s" key

![image](https://github.com/user-attachments/assets/b15df673-320c-476a-9d7a-b615a1d71f53)


5.Identified VPwR from the layout using "s" key

![image](https://github.com/user-attachments/assets/67eecf96-f968-41de-9ea8-940f55dedf51)


6.Identified Ground(VDD) from the layout using "s" key

![image](https://github.com/user-attachments/assets/8ddaa436-2eb5-47b6-87e3-ea0a25abe250)


7.Extracting spice file of inverter layout file using tkcon command line

![image](https://github.com/user-attachments/assets/3b1d1494-f8dc-4670-9dcd-0613712c5b67)



8.Extracted SPICE file screenshot in vim

![image](https://github.com/user-attachments/assets/ae6cdbef-1607-4067-9189-ad43a17e3e78)



<h3>9.After making some required changes in the SPICE file:</h3>
  <li>Changing the load capcitance to remove the spikes during transition</li>
 <li>Adding values for Pulse(VPULSE) </li>
 <li>Adding VDD and VSS values</li>
 <li>Adding details about the analysis to perform</li>
<br/>
<br/>

10.Running NGSPICE for charaterisation

<img>![image](https://github.com/user-attachments/assets/aff80527-c64f-4c98-820e-324652d8990d)</img>


11.Plots obtained from NGSPICE
As you can see the spikes during the transistion time

![WhatsApp Image 2024-12-11 at 22 13 48_09c52467](https://github.com/user-attachments/assets/cb0fbc1e-6ef1-4b8c-835c-c95228fc1e02)

12.Plot obtained after changing the load capacitance
We can observe that the spikes have been smoothened out due the changes in load capacitance

![WhatsApp Image 2024-12-11 at 22 18 52_1ef37f46](https://github.com/user-attachments/assets/272b86f9-6b29-4396-8cda-38d0b0d20885)

<h3>13.Rise time calculatios</h3>
<p>20% graph plot</p>

![WhatsApp Image 2024-12-12 at 12 41 12_3a90a9d7](https://github.com/user-attachments/assets/2a64f5d7-77dd-4e4d-ac70-a7e20ab254b4)

<p>80% graph plot</p>

<img>![WhatsApp Image 2024-12-12 at 12 42 33_5a5c0b4a](https://github.com/user-attachments/assets/2cdfa141-2e98-4b2a-98e2-4e3ee4ee7ca1)</img>

<p>Value of the points obtained from the above two plots</p>

<img>![WhatsApp Image 2024-12-12 at 12 44 06_a340f83d](https://github.com/user-attachments/assets/771c8c75-fea0-4d9d-a0bf-cfd3714cf402)</img>

<p>Calculation of Rise Transition Time</p>

<img>![WhatsApp Image 2024-12-12 at 12 46 42_3d44cb76](https://github.com/user-attachments/assets/bebbdeb9-56d0-4856-9bba-05fd554b42bc)</img>

<h3>14.Rise cell delay calculations</h3>
<p>50% graph plot</p>

<img>![WhatsApp Image 2024-12-12 at 13 37 43_e6d3fbb1](https://github.com/user-attachments/assets/33261c95-1409-4561-b35a-6429bb96f350)</img>

<p>Calculations of Rise Cell delay with obtained values</p>

<img>![WhatsApp Image 2024-12-12 at 13 39 20_0103fc4b](https://github.com/user-attachments/assets/b14274ee-1f23-4b0d-ac8e-6c7809f39d1c)</img>

<h3>15.LAB Challenge of correcting DRC rules using skywater 130nm documentation</h3>
<p>Downloading the files,Unziping it and listing the obtained files done on the following screenshot.</p>

<img>![WhatsApp Image 2024-12-12 at 13 44 31_eb04256b](https://github.com/user-attachments/assets/a2e4e94b-d8cc-4d61-a99d-14196ac892de)</img>

<p>Screenshot of the .magicrc file</p>

<img>![WhatsApp Image 2024-12-12 at 13 53 03_c3694a95](https://github.com/user-attachments/assets/6e1c549e-89b8-4d73-aef8-39c0f369e8f2)</img>

<p>Command run on the terimanl to open the magic window</p>

<img>![WhatsApp Image 2024-12-12 at 13 55 09_3742754d](https://github.com/user-attachments/assets/12b11e6e-949d-4484-8295-47b9f263a02d)</img>

<p>Screen shot of the Magic window and checking the DRC rule violation using <br/>
 <code>drc why</code>
</p>

<img>![WhatsApp Image 2024-12-12 at 13 56 51_bb6af292](https://github.com/user-attachments/assets/5505d78a-38e8-434e-9cc0-c2896fc5630d)</img>

<p>Verifying the Edge rule violation using the <code>box</code> command </p>

<img>![WhatsApp Image 2024-12-12 at 14 54 03_6d15f27c](https://github.com/user-attachments/assets/d98bb1a9-ff12-4d7b-850e-c040ecdde8be)</img>

<p>Inserting metal contact in grid fashion using the tkcon window</p>

<img>![WhatsApp Image 2024-12-12 at 14 58 35_b147937e](https://github.com/user-attachments/assets/4542116b-215a-4d35-b40b-c2a7b5b3e21d)</img>

<p>Successfully identifying <i>npolyres</i> and <i>poly</i> mask layer using tkcon window</p>

<img>![WhatsApp Image 2024-12-12 at 15 02 17_265e3cb1](https://github.com/user-attachments/assets/41427403-8118-4ead-8551-6d592cb1355d)</img>

<h4>The correction of various DRC rules executed in the program for illustration purpose was successfully implemted,but the screenshots were not recovered properly.</h4>


</p>
</details>
<h2>Pre-layout timing analysis and importance of good clock tree</h2>
<details>
<summary>Day 4 </summary>
<p>
 <p>Changing the grid size according to the metal tracks dimensions</p>

<img>![WhatsApp Image 2024-12-12 at 15 05 28_d44d7e4e](https://github.com/user-attachments/assets/54e1580f-5a25-4675-ac8c-8d2e7113b608)</img>

<p>Screenshot of the changed grid size in Magic window</p>

<img>![WhatsApp Image 2024-12-12 at 15 08 33_584b93c2](https://github.com/user-attachments/assets/bee84c8c-e1d1-4e98-b9dd-29dae3080b9f)</img>

<img>![WhatsApp Image 2024-12-12 at 15 10 26_96678695](https://github.com/user-attachments/assets/4d829027-fcb8-4344-afd6-4d12a4d99ec5)</img>

<p>We verified the following coniditions are met to fix the DRC error and verify that the design ready to be plugged into the flow</p>
<li>The input and output ports of the standard cell should lie on the intersection of the vertical and horizontal tracks.</li>
<li> Width of the standard cell should be odd multiples of the horizontal track pitch.</li>
<li>Height of the standard cell should be even multiples of the vertical track pitch.</li>
<br/>

<p>Saving the layout file of Magic window using </p>

<code>save sky130_vsdinv.mag</code>
<br/>

<img>![WhatsApp Image 2024-12-12 at 15 10 07_20205ebe](https://github.com/user-attachments/assets/d8f5fc76-af0b-42c8-8496-089b18924718)</img>

<p>Creating a LEF file from the layout file using the command</p>
<code>lef write</code>

<img>![WhatsApp Image 2024-12-12 at 15 15 26_50e13b4e](https://github.com/user-attachments/assets/075bcc62-897d-4f84-8d71-21a07a4f2e69)</img>

<p>Verifying the creation of the LEF file using the terminal</p>

<img>![WhatsApp Image 2024-12-12 at 15 19 33_f3016a3a](https://github.com/user-attachments/assets/6ce6498c-d124-483a-90e4-e0efcafd4079)</img>

<p>Screenshot of the content of the generated LEF file</p>

![WhatsApp Image 2024-12-12 at 15 21 31_e39886e0](https://github.com/user-attachments/assets/d47e978d-72c6-4cff-80be-443225a728e6)

<p>Content of the picorv32a/src folder before copying the generated file</p>

![WhatsApp Image 2024-12-12 at 15 44 07_d17ce197](https://github.com/user-attachments/assets/ef02c956-c4a0-41a8-8512-a7486aadadd3)

<p>Verification of the contents of the <code>picorv32a/src</code> directory </p>

![WhatsApp Image 2024-12-12 at 15 48 23_869a1b00](https://github.com/user-attachments/assets/28b8c179-f4a0-43ff-9033-f73f42d42e30)

<p>Changes made in the config.tcl file to change the lib file and add new lef files into the OPENLANE flow</p>

```bash
 set ::env(LIB_SYNTH) "$::env(OPENLANE_ROOT)/designs/picorv32a/src/sky130_fd_sc_hd__typical.lib"
set ::env(LIB_FASTEST) "$::env(OPENLANE_ROOT)/designs/picorv32a/src/sky130_fd_sc_hd__fast.lib"
set ::env(LIB_SLOWEST) "$::env(OPENLANE_ROOT)/designs/picorv32a/src/sky130_fd_sc_hd__slow.lib"
set ::env(LIB_TYPICAL) "$::env(OPENLANE_ROOT)/designs/picorv32a/src/sky130_fd_sc_hd__typical.lib"

set ::env(EXTRA_LEFS) [glob $::env(OPENLANE_ROOT)/designs/$::env(DESIGN_NAME)/src/*.lef]
```

![WhatsApp Image 2024-12-12 at 15 55 49_6caa3408](https://github.com/user-attachments/assets/e9f55efb-8066-4a86-a035-f9a80a6577c6)

<p>Opening OPENLANE using <code>docker</code> command and starting an interactice session using <code>./flow.tcl -interactive</code> </p>

![WhatsApp Image 2024-12-12 at 16 01 27_f5668447](https://github.com/user-attachments/assets/91e8fbbb-94b3-4df8-886e-16ee6ddc1833)

<p>Error I faced and I corrected it by replacing</p>
<li>LIB_MAX with LIB_SLOWEST </li>
<li>LIB_MIN with LIB_FASTEST</li>
<br/>

![WhatsApp Image 2024-12-12 at 16 03 49_533aca80](https://github.com/user-attachments/assets/519c48c2-d15e-4b79-b07c-c5071052c306)

![WhatsApp Image 2024-12-12 at 16 03 49_533aca80](https://github.com/user-attachments/assets/43ea8ce5-1546-4b74-b847-184ada9792e6)

<p>Screenshot of successfully running <code>prep -design picorv32a</code> command </p>

![WhatsApp Image 2024-12-13 at 00 20 29_780c38b4](https://github.com/user-attachments/assets/a0e8783f-4e07-4d22-879e-a44c85726701)

<p>Screenshot of successfully running <code>run_synthesis</code> command </p>

![WhatsApp Image 2024-12-13 at 00 24 00_d0a7602e](https://github.com/user-attachments/assets/f71b0a15-bb77-44b3-880f-7c68feb564d5)

<p>Examing and setting various variables related to SYNTH_STRATERGY and SYNTH_SIZING and SYNTH_DRIVING _CELL</p>

![WhatsApp Image 2024-12-13 at 00 26 36_df4fbba2](https://github.com/user-attachments/assets/af85337d-cf1f-4fe3-8e26-e03919dde486)

<P>Errors faced during <code>run_floorplan</code> which was later corrected </P>

![WhatsApp Image 2024-12-13 at 00 30 08_31b892db](https://github.com/user-attachments/assets/1d3008ba-14d3-4af7-b400-205d6a3bab37)

<p>Screenshot of the <code>run_placement</code> command </p>

![WhatsApp Image 2024-12-13 at 00 31 53_a6270b14](https://github.com/user-attachments/assets/56bb771c-259e-42d3-a169-df701cf2a9d6)

<p>Screemshot of the DEF in magic </p>

![WhatsApp Image 2024-12-13 at 00 35 12_97863266](https://github.com/user-attachments/assets/82053033-12df-4b1a-a737-e80bcbbf3762)

<p>Screenshot of custom inverter inserted in placement DEF with proper abutment</p>

![image](https://github.com/user-attachments/assets/6ced1baa-ebff-49f3-bce7-98ebc7802d89)

<p>Screenshot of proper abutment of power pins with other cell from library</p>

![image](https://github.com/user-attachments/assets/13323af3-52ff-4fdd-91eb-52b794cec97c)









</p>
</details>
<h2>Final steps for RTL2GDS using tritonRoute and openSTA</h2>
<details>
<summary>Day 5 </summary>
<p>Your content goes here.</p>
</details>
