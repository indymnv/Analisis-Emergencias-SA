# Analisis-Emergencias-SA
From June 2020 until today, I work part-time as a consultant analyst for the San Antonio Fire Department, where one of my jobs is to report the development of emergencies over time. Here I show a small script that I developed to analyze emergencies with Python, using the classic libraries such as Pandas, Matplotlib, etc. 
# Context
The Fire Department has four stations that operate in a specialized way to control some emergencies. However, they also collaborate according to the emergency they are addressing. This guideline is subject to a dispatch pattern that may vary over time but based on the places where the companies are located and the emergencies that arise. The variables shown are the following:

Name | Meaning
------------ | -------------
Date | Corresponds to the date of the call
Time of call | It corresponds to the time of the call
Time of the first reply | It corresponds to the time the first car arrives
Type of Emergency | If it is fire, rescue, etc. The meaning of the acronyms is detailed later.
Address | Corresponds to the direction of the emergency
1cia | x if and only if the First Company attends the emergency, 0 otherwise
2cia | x if and only if the Second Company attends the emergency, 0 otherwise
3cia | x if and only if the Third Company attends the emergency, 0 otherwise
4cia | x if and only if the First Company attends the emergency, 0 otherwise
Emergency end time | Time that Firefighters controlled emergency
Situation | Description of the emergency

The emergency codes are as follows:

* 10-0 Structural Fire
* 10-1 Vehicle Fire
* 10-2-1 Grassland and/or garbage fire in urban forest interface.
* 10-2-2 Forest fire.
* Forest fire alarm (support unit Z-0, B-4 + Water unit)
* 10-3-1 Support to SAMU or Animal Rescue.
* 10-3-2 Technical rescue on unevenness (ravine, elevators, cliff, well, ditch, roofs).
* 10-3-3 Rescue in collapsed structures
* 10-4-1 Vehicle rescue, Private transportation.
* 10-4-2 Vehicle rescue, passenger transportation (buses, buses, school transports).
* 10-4-3 Vehicle rescue, cargo vehicles, heavy machinery (trucks, cranes, heavy-duty machinery).
* 10-5-1 Fuel spill, hydrocarbon derivatives, minor spill.
* 10-5-2 Hazardous materials, with household products.
* 10-5-3 Hazardous materials during transportation (train, truck, ship).
* 10-5-4 Hazardous materials in industries (port companies, storage warehouses)
* 10-6-1 Possible gas leak in private homes
* 10-6-2 presumable gas leak in places with a high influx of public (commercial premises, schools, department, local gas sales)
* 10-7 Electric call.
* 10-8 Unclassified call.
* 10-9 Call to other services. No emergency.
* 10-10 Call for removal of debris or regrowth
* 10-12 Call to support other Fire Brigades
* 10-15 simulacrum

