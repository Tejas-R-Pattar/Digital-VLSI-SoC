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
![WhatsApp Image 2024-12-11 at 19 58 57_b808f40a](https://github.com/user-attachments/assets/0a24c115-efe2-47e3-9049-490dd44c09a7)


8.Extracted SPICE file screenshot in vim
![WhatsApp Image 2024-12-11 at 19 59 45_f39d27ef](https://github.com/user-attachments/assets/1e20114c-760a-41d5-a23f-ef25a436a2b3)


9.After making some required changes in the SPICE file:
-Changing the load capcitance to remove the spikes during transition
-Adding values for Pulse(VPULSE) 
-Adding VDD and VSS values
-Adding details about the analysis to perform
 
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
