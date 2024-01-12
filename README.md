# IVAD
In-vehicle attack dataset
The In-Vehicle Attack Dataset (IVAD) is an intrusion detection dataset used to train in-vehicle IDS. It comprises a total of four files, corresponding to datasets with 1, 3, 5, and 7 CAN IDs, respectively. The data on the CAN bus in these files has been converted from hexadecimal to decimal format.

The core of IVAD was collected from the real Smart #1 vehicle. To enhance the variety of attacks in the IVAD, spoof attacks such as gear/RPM from the CHD and malfunction attacks from the SAD were extracted and incorporated into IVAD. Furthermore, to align with the cloud-vehicle collaborative detection environment, we collected data (include normal, DoS attack, fuzzy attack and replay attack) from a cloud-vehicle collaborative simulation environment.

The interpretation of the feature columns in the file is as follows:

CANID：The ID segment carries information about the source and priority of a message. It distinguishes different types of messages and facilitates message filtering.  
Data1-8：The Data segment contains the actual payload or information that is being transmitted. This segment can vary in size, depending on the DLC value specified in the previous segment.  
Label：The label of the traffic is used to differentiate whether the flow is malicious or not. Here, ‘1’ represents an malicious message while ‘0’ represents a normal message.  

The classifications and quantities of attacks included in IVAD are illustrated as follows:
--------------------
Nomal: 2542535  
DoS attack: 587521  
Fuzzy attack: 590531  
Replay attack: 96357  
Gear Spoof attack: 597252  
RPM Spoof attack: 654897  
Malfunction attack: 15974  
Total 5085067
---------------------------


