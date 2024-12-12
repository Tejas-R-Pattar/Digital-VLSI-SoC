<details>
<summary> Day-1 Inception of open-source EDA, OpenLANE and Sky130 PDK </summary>
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
<details>
<summary> Day-2 Good floorplan vs bad floorplan and introduction to library cells</summary>
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
<details>

<summary>Day 3  Design library cell using Magic Layout and ngspice characterization</summary>
<p>
1.Git cloning custom inverter standard cell design from github repository of Nickson Jose sir 


2. Viewing inverter in magic and also the console for other interactions
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
<img>![WhatsApp Image 2024-12-12 at 12 41 12_3a90a9d7](https://github.com/user-attachments/assets/2a64f5d7-77dd-4e4d-ac70-a7e20ab254b4)</img>

<p>80% graph plot</p>
<img>![WhatsApp Image 2024-12-12 at 12 42 33_5a5c0b4a](https://github.com/user-attachments/assets/2cdfa141-2e98-4b2a-98e2-4e3ee4ee7ca1)</img>

<p>Value of the points obtained from the above two plots</p>
<img>![WhatsApp Image 2024-12-12 at 12 44 06_a340f83d](https://github.com/user-attachments/assets/771c8c75-fea0-4d9d-a0bf-cfd3714cf402)</img>

<p>Calculation of Rise Transition Time</p>
<img>![WhatsApp Image 2024-12-12 at 12 46 42_3d44cb76](https://github.com/user-attachments/assets/bebbdeb9-56d0-4856-9bba-05fd554b42bc)</img>



</p>
</details>
<details>
<summary>Day 4 </summary>
<p>Your content goes here.</p>
</details>
<details>
<summary>Day 5 </summary>
<p>Your content goes here.</p>
</details>
