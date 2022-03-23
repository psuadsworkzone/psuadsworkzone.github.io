# Safe Integration of Automated Vehicles into Work Zones.
Welcome to the Penn State wiki page for details on the Automated Driving System Workzone project. This page presents details primarily focused on the Penn State team activity. Additional details can be found at the PennDOT's public ADS page, which can be found [here](https://www.penndot.gov/ProjectAndPrograms/ResearchandTesting/Autonomous%20_Vehicles/Pages/ADS-Demonstration.aspx)

# The Motivation for the Safe Integration of Automated Vehicles into Work Zones
***
In 2015 there were an estimated 96,626 crashes in work zones, an increase of 7.8 percent from 2014. This makes 2015 the second year in a row that work zone crashes rose after a low of 67,887 in 2013.  For comparison, in 2009 there were 667 work zone fatalities. Crashes in highway work zones have killed at least 4,700 Americans – more than two a day – and injured 200,000 in the last five years alone. There are more than 40,000 injuries in work zones each year. About 85 percent of people killed in work zones are motorists, not workers.

In Pennsylvania, the number of work zone crashes has steadily increased since 2007. Pennsylvania has also consistently appeared in the top 10 states with the most commercial motor vehicle-related work zone crashes. 

With Autonmous Vehciles being increasingly deployed to public roads, construction zones may present challenges to these vehicles, construction zone operators, and the surrounding traffic. Construction zones, by definition, are new areas with features that did not exist earlier, that are dynamic, and that may not follow typical conventions. The AV behaviors in workzones may not follow human-driven vehicle behavior, which can confuse construction zone operators that may assume human driving behavior. And as both AVs and construction environments interact with each other, the vehicles nearby the AV may also need to respond to new behaviors. Our project intends to investigate these behaviors to improve safety in and around work zones for AVs. This is achieved by increasing identification and connectivity with work zone artifacts, improving visibility by coating pavement marking and work zone artifacts, and improving mapping of work zones.

# Project Vision, Mission, Goals, and Objectives
***
Vision – Enable automated vehicles to safely operate in work zones without human intervention.

Mission – Reduce traffic fatalities and increase mobility for all Americans in work zones through automated vehicles.

Goals – Achieve safe navigation of automated vehicles on par with non-distracted, humanoperated automated vehicles within work zones.

Objectives of this project:
1. Evaluate the impact of improved connectivity between the AVs and the work zone artifacts using DSRC/C-V2X.
2. Evaluate the impact of increased visibility (machine vision) of pavement markings and work zone artifacts on AVs through innovative coatings
3. Evaluate the impact of providing high definition mapping of work zone artifacts (i.e. cones, barrels, workers, vehicles)
4. Improve the map information dissemination process from the mapping providers and/or infrastructure owners/operators to the AVs through standardization of digital mapping information for work zones.
# Task list
***
## Year 1:
Prepare mapping van systems for field testing including:
* Time synchronization
* Camera mounting
* Camera calibration
* LiDAR install
* Data parsing
* Image stitching
etc.

Prepare V2x systems for comms

Prepare road-side devices for connectivity and position measurement

Prepare CARLA computers

Develop code to import mapped environment into CARLA

Develop code to parse mapping van data for work-zone objects

Develop code that determines safety metrics for work zones

(etc).

# Team members (Penn State Only)
***
 
* Project PIs
  
  Dr. Sean Brennan  
<img src="https://github.com/ForgetfulDatabases/ForgetfulDatabases.github.io/blob/main/assets/images/brennan-sean_2017.jpg?raw=true" height = "260" width= "200">  

 


 * Students

 Maddipatla Satya Prasad   |  Wushuang Bai             | Liming Gao                | Xinyu Cao
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
<img src ="https://github.com/psuadsworkzone/psuadsworkzone.github.io/blob/main/SatyaPrasadMaddipatla.jpg?raw=true" height = "200" width= "200">  |<img src="https://github.com/psuadsworkzone/psuadsworkzone.github.io/blob/main/WushuangBai_photo.jpg?raw=true" height = "200" width= "200"> | <img src="https://user-images.githubusercontent.com/66030812/148875266-8b5677b8-01df-46fd-8fbd-e02e0ea36858.jpg?raw=true" height = "200" width= "200"> |  <img src="https://github.com/psuadsworkzone/psuadsworkzone.github.io/blob/main/XinyuCao.jpg?raw=true" height = "200" width= "200">

# Testing vehicles
***
* Penn State Mapping Vehicle
See [https://connectedvehicles.psu.edu/](https://connectedvehicles.psu.edu/)
<br>

* CMU's AV vehicle fleet
<br>


# Data flow 
***
The data flows through sensors on the vehicle, computational systems in the vehicle, hard drives, computational systems off-vehicle, local databases/servers, cloud service, and finally goes into applications such as autonomous vehicles, vehicle simulation such as CARLA, traffic simulation such as SUMO and other end users. A high leve view of the data flow is shown as below.

<img src="https://github.com/psuadsworkzone/psuadsworkzone.github.io/blob/main/DataFlowHighView.png?raw=true" > 

The mapping vehicle is instrumented with GPS, Cameras, LiDAR, Encoder, IMU and Road Wheel Angle String Potentiometers. We do calibration after vehicle building, and before and after tests to secure data quality. 

<img src="https://github.com/psuadsworkzone/psuadsworkzone.github.io/blob/main/SensorBuildingAndCalibration.png?raw=true" > 

We use a multi-database architecture to process the data.

![](./DataFlow.PNG)

The data finally can be delivered to end users such as autonomous vehicles, vehicle simulation such as CARLA, traffic simulation such as SUMO.

<img src="https://github.com/psuadsworkzone/psuadsworkzone.github.io/blob/main/DataDelivery.PNG?raw=true" > 




# Code repositories
***
Code repositories are hosted by IVSG as below.

| Category                             | Description                                                                                      | Repo address                                                                                                         |
|--------------------------------------|--------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| Documents                            | Mapping vehicle calibration data and results                                                     | https://github.com/ivsg-psu/Hardware_MappingVanHardware_Calibration                                                  |
| Documents                            | Mapping vehicle set up information, such as wiring layouts, physical   locations of sensors, etc | https://github.com/ivsg-psu/Hardware_MappingVanHardware_HardwareSummary                                              |
| Documents                            | GPS information on the mapping vehicle.                                                          | https://github.com/ivsg-psu/Hardware_MappingVanHardware_GPS                                                          |
| Documents                            | Camera information on the mapping vehicle.                                                       | https://github.com/ivsg-psu/Hardware_MappingVanHardware_Camera                                                       |
| Documents                            | LiDAR information on the mapping vehicle.                                                        | https://github.com/ivsg-psu/Hardware_MappingVanHardware_LiDAR                                                        |
| Documents                            | Encoder information on the mapping vehicle.                                                      | https://github.com/ivsg-psu/Hardware_MappingVanHardware_Encoder                                                      |
| Documents                            | IMU information on the mapping vehicle.                                                          | https://github.com/ivsg-psu/Hardware_MappingVanHardware_IMU                                                          |
| Documents                            | Steering system information on the mapping vehicle.                                              | https://github.com/ivsg-psu/Hardware_MappingVanHardware_SteeringSystem                                               |
| Code - calibration                   | Cameras calibration                                                                              | https://github.com/ivsg-psu/FieldDataCollection_TypicalHardwareSetups_CameraCalibration                              |
| Code - calibration                   | Camera-to-LiDAR calibration                                                                      | https://github.com/ivsg-psu/FieldDataCollection_TypicalHardwareSetups_CameraToLiDARCalibration                       |
| Code - calibration                   | Steering system calibration                                                                      | https://github.com/ivsg-psu/FieldDataCollection_TypicalHardwareSetups_SteeringCalibration                            |
| Code - calibration                   | Vehicle dynamics calibration                                                                     | https://github.com/ivsg-psu/FieldDataCollection_TypicalHardwareSetups_VehicleDynamicsCalibration                     |
| Code - test                          | Code to operate sensors on mapping vehicle                                                       | https://github.com/ivsg-psu/FieldDataCollection_DataCollectionProcedures_MappingVanROSNodes                          |
| Code - post test data processing     | Code for step "Parse and Push"                                                                   | https://github.com/ivsg-psu/FieldDataCollection_DataCollectionProcedures_ParseRawDataToDatabase                      |
| Code - post test data processing     | Code for step "Data Clean"                                                                       | https://github.com/ivsg-psu/FeatureExtraction_LaneDetection_LIDAR_Reflectivity_And_Geometry_Lane_Extraction          |
| Code - post test data processing     | Code for step "Associate with Map"                                                               | https://github.com/ivsg-psu/FieldDataCollection_DataCollectionProcedures_MapAssociation                              |
| Code - post test data processing     | Code for step "Merging of    maps"                                                               | https://github.com/ivsg-psu/FieldDataCollection_DataCollectionProcedures_MapMerge                                    |
| Code - post test data processing     | Code for generating "Reference template"                                                         | https://github.com/ivsg-psu/FieldDataCollection_DataCollectionProcedures_ReferenceTemplateGeneration                 |
| Code - data delivery to applications | Code for step "Data delivery"                                                                    | https://github.com/ivsg-psu/FieldDataCollection_DataCollectionProcedures_AutomatingDataTransferToDMSUsingCommandLine |
| Code - data delivery to applications | Code for converting data into format following OpenDrive standard                                | https://github.com/ivsg-psu/FieldDataCollection_RoadSegments_ExportingOpenDRIVEfromMATLAB                            |
| Code - data delivery to applications | Code for setting up CARLA simulator                                                              | https://github.com/ivsg-psu/DrivingSimulators_VirtualEnvironment_SetupCARLA                                          |
| Code - data delivery to applications | Code for importing customized maps into CARLA                                                    | https://github.com/ivsg-psu/DrivingSimulators_VirtualEnvironment_SetupCARLA                                          |

# Equipment inventory
We have received traffic objects from PennDOT as below.
![](./TrafficObjectsReceivedFromPennDOT.PNG)
We also have traffic objects hosted by Penn State that we can use on test track.
![](./TrafficObjectsHostedByPennState.PNG)

# Penn State activities
***
We set up an example data structure in the DMS to validate the directory as per task 2.1.

<img src="https://github.com/psuadsworkzone/psuadsworkzone.github.io/blob/main/DataStructureInDMS.png?raw=true" > 

We did a test run to validate the mapping vehicle operation.

<img src="https://github.com/psuadsworkzone/psuadsworkzone.github.io/blob/main/exampleMappingImage.jpg?raw=true" > 

We started to test the CARLA traffic simulator.

<img src="https://github.com/psuadsworkzone/psuadsworkzone.github.io/blob/main/CARLATest.png?raw=true" > 
# Broader impacts 
***
The Automated Driving System Work Zone reduces abnormal vehicle behaviors improves safety by providing information to the AVs in real-time. By creating the connection between the AVs and construction environments, reliable and accurate information can be used by AVs to make decisions when approaching and driving through work zones. By investigating the behaviors resulting from these decisions, we not only can improve safety in and around work zones for AVs but also the safety of construction zone operators and other motorists. Apart from that, in combination with traffic flow in this area, these behaviors can also be used to adjust the layout of the working zone to ease congestion and inform motorists at an appropriate time and location to improve time and cost effectiveness.

# Groups with related interests
***
Please see links below for other research groups with related interests:
<ul>
<li>
 <a href = "https://ctre.iastate.edu/roadway-information-database-rid/">
  SHRP 2 WEBINAR: SHRP 2 Roadway Information Database (RID): Doing Research without NDS data.
 </a>
</li>
 <li>
 <a href = "https://carla.org/">
  CARLA - Open-source simulator for autonomous driving research.
 </a>
</li>
  <li>
 <a href = "https://www.plm.automation.siemens.com/global/en/products/simcenter/prescan.html">
  PreScan - Develop more reliable and safer automated vehicle functionalities.
 </a>
</li>
   <li>
 <a href = "https://www.eclipse.org/sumo/">
  SUMO - n open source, highly portable, microscopic and continuous multi-modal traffic simulation package designed to handle large networks.
 </a>
</li>
 
    <li>
 <a href = "https://www.transportation.gov/policy-initiatives/automated-vehicles/36-pennsylvania-department-transportation">
  Funding information by USDOT. 
 </a>
</li>
 
     <li>
 <a href = "https://www.mathworks.com/products/roadrunner.html">
  RoadRunner - Design 3D scenes for automated driving simulation.
 </a>
</li>
 
  <li>
 <a href = "https://www.mathworks.com/">
  MATLAB for Artificial Intelligence.
 </a>
</li>
 
   <li>
 <a href = "https://www.commsignia.com/">
  Commsignia connects cars with each other and the smart city infrastructure for a safer, more efficient and more sustainable transportation.
 </a>
</li>
</ul>


# Funding
This project is funded by USDOT via Pennsylvania Department of Transportation under NOFO # 693JJ319NF00001.

