---
layout: page
title: picoGreen DNA Quantification Assay for dsDNA (IN REVISION)
bigimg: /img/tapestation.JPG
---

## Background
The picoGreen Quantification Assay provides an easy and relatively inexpensive way to quantify the concentration of DNA a single sample or scale up to whole plate quantification. It does this via a flourscences based technique, and works similar to a broad spectrum DNA Qubit Assay, but can be performed on plates making it more ideal for large sample sizes.

## Equipment & Reagents
* Plate Reader 
* Standard 10ul Tips (one per sample)    
* Standard 200ul tips      
* Black 96 well plate   
* PicoGreen Assay Kit:                                            
   * | Reagent | Amount | Concentration | Storage | Stability | 
     |:-------:|:------:|:-------------:|:-------:|:---------:|
     | Quant-iT™ PicoGreen® dsDNA reagent (stored at < 8C) | 1 mL | Solution in DMSO | 2-6C | 6 months |
     | 20X TE | 25 mL | 200 mM Tris-HCl, 20 mM EDTA, pH 7.5 | Room Temp | 6 months |
     | Lambda DNA standard | 1 mL | 100 μg/mL in TE | 2-6C | 6 months |


![](https://github.com/adowneywall/Tutorials/blob/master/img/Gen5%203.03%20-%20Experiment1_%20%5Bcreated%20from%20dsDNA%20picogreen%20assay%20full%20plate.prt%5D%207_5_2019%2010_44_00%20AM.mp4)

## Important Notes **READ BEFORE USING**: 
* Samples are run along side a set of 6 standards (including blank). These standards will need space on plate you are prepping. The manual doesn't specifically mention if a unique set of standard are required for each plate prepared, but I tend to included them on each plate to serve as replicate readings for the standards in order to increase confidence in the the measurements. The easiest thing to do is dedicate the first column of the plate for standards. However, this may not be necessary if you are looking to only use the minimum amount of each reagent.

## Things to do before starting

**30 minutes ahead of time**
* Take the Quant-iT™ PicoGreen® dsDNA reagent out of the refridgerator, it will be solid at 8C at refridgerator temperature.

**5 minutes ahead of time (or more)**
* Turn on the synergy plate read using the power button on the front left of the unit and log on to the attached computer (login info taped to the computer). 

**Insert Picture**

## Protocol

### Step 1 - Dilute 20X TE and Quant-iT™ PicoGreen® dsDNA reagent

Both 20X TE and the picoGreen reagent will need to be diluted before there use. The 20X TE is created **first** (you'll need to do the picoGreen dilution), and you will generally need a sterile 50mL vial for your dilution (this will depend on the number of samples you are running). The 1X TE is created using mol. grade grade water using the formula below. Next, the picoGreen reagent diltution is performed using the 1X TE dilution you just created with the formula below. The 1.1 in the formula is used to add a 10% solution buffer to account for pipetting error. 

**1X TE Stock Calculation**

Determine amount of 1X TE you will need: 
1.1*(50uL 1X TE x Number of samples + (271uL x Number of plates)) = 1X TE Total volume (ul)
* Total volume 1X TE / 20 = **20X TE volume (ul)** 
* 20X TE volume (ul) * 19 = **Mol. Grade Water (ul)**

**picoGreen Dilution Calculation**

Determine amount of diluted picoGreen you need:
1.1*(50uL diluted picoGreen x Number of samples + (300uL x Number of plates)) = picoGreen Diluted Total Volume (ul)
* Total volume diluted picogreen / 200 = **Stock picoGreen (ul)**
* picoGreen Stock (ul) * 199 = **Mol. Grade Water (ul)**

### Step 2 - Creating Dilution stocks for standards 

Standards are created by before a serial dilution using a provided ladder. They can be created following the table below. 

| Dilution Created       | Dilution Used |  Volume | 1X TE | Total |
|:----------------------:|:-------------:|:-------:|:-----:|:-----:|
| Dilution 1 (2ug/ml)    | Stock ladder (100ug/ml)  | 1uL     | 49uL  | 50uL  |
| Dilution 2 (0.2ug/ml)  | Dilution 1    | 5uL     | 45uL  | 50uL  |
| Dilution 3 (0.02ug/ml) | Dilution 2    | 5uL     | 45uL  | 50uL  |

* Note: 17.5 uL of Dilution 1, 7 uL of Dilution 2, and 5 uL of Dilution 3 **per plate** since you should run your standard for every plate.

### Step 2 - Loading the plate for reading 

* Both standards and samples have a total reaction volume of 100uL. The composition of the reactions is indicated in the tables below.
* Standard and samples can be arranged however you like, but the standard layout is to use the first column for standardes and the remaining 11 columns for samples (88 samples). **NOTE**: you will need to match the layout of the plate with the digital plate on the plate reader GUI to make sure 

**Standards Reactions**

| Standard_ID | Conc. (ng/ml) | Ladder Dilution (ug/ml) | Ladder Volume (ul) | 1X TE Volume (ul) | Diluted PicoGreen Volume (ul) |
|:-----------:|:-------------:|:-----------------------:|:------------------:|:-----------------:|:-----------------------------:|
| 1   |	500    |	Ladder Dilution 1 (2ug/ml)   |  25   | 25    | 50    |
| 2   |	250    |	Ladder Dilution 1 (2ug/ml) |  12.5   | 37.5    | 50    |
| 2   |	100    |	Ladder Dilution 1 (2ug/ml) |  5   | 45    | 50    |
| 3   | 25     | Ladder Dilution 2 (0.2ug/ml)  |  25  | 25    | 50    |
| 5   | 5      | Ladder Dilution 3 (0.02ug/ml)  |  25   | 25    | 50    |
| 6   | Blank  | Blank                         | -    | 50   | 50    | 

**Sample Reaction**

| Sample | 1X TE | PicoGreen Dilution | Total  |
|:------:|:-----:|:------------------:|:------:|
| 1uL    | 49uL  | 50uL               | 100uL  |

### Step 3 - Running Synergy Plate Reader

**Step-wise Instructions**
1) Open Gen5 3.03 software
2) Make sure the plate reader is turned on. Switch is on the front left.
3) When the 'Task Manager' window pops up select the 'dsRNA_protocol_assay.prt' under Recent options
4) Select the 'Plate Layout' option on the task bar.
5) This will bring up a separate window that has a Plate schematic (a 8x12 matrix) that represents locations on the plate.
6) The first column should have the 6 standards (5 with 250,100,10,4,1 ug/ml and a blank) positioned in rows B-G.
7) Since running a full plate the remaining cells on the plate have randomly incremented sample ids. Note: these could be the actual well_IDs if prepped ahead of time.
8) Load the 96-well plate in the plate reader.
9) Press the green arrow on the task bar, then highlight the entire plate when the plate window appears. Click "OK" to begin the analysis.
10) This reading should take approximately 20 seconds.

### Step 4 - Storing Data and Adjusting Calculations 

TO DO
