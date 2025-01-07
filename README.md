# BMW-E-Series-Remote-Start
( STILL IN DEVELOPMENT STAY TUNED ) ( INFO OR TUTORIAL MIGHT NOT BE COMPLETE )

Im open for sugestions for features and help if anyone wants :)

Exact tutorial will be made when the code is done ( still making it at the moment )

COMPATIBLE ONLY WITH CAS2 AND CAS3 SYSTEMS ( ANYTHING OLDER AND NEWER WONT WORK )

Remotely start all E series cars with manual transmission with the help of an app or Bluetooth beacon or fingerprint.

Based on arduino nano ble 33 rev2

Fully designed in case of failure or arduino looses power it reverts to the original system

For the remote start features to work we need some info and some parts from the car for status and safety

Info required from car ( for safety )

Hall sensor for ( Shifter neutral detection ) ( this will normaly attach on the shaft of the transmission and detect the position with a magnet )
Clutch sensor   ( for the cars that have a clutch sensor to start the arduino will simulate the clutch being pressed ) ( and monitor the sensor for stall detection
Driver door detection ( for future uses ) ( still thinking if it can be useful )
Rpm Detection ( to avoid the car being turned off the arduino checks the rpm ) ( if rpm is not in idle 900-1000 it wont allow to turn off the engine ) only original system can do that
Parking brake detection( if the parking brake is not on the arduino wont allow remote start )
Battery voltage detection ( if the battery is low the arduino wont allow remote start ) ( still thinking if i take from the canbus the info or with resistor devider )
Canbus detection ( to reterive the door status and rpm from the K-CAN of the car )

Parts required

Arduino nano 33 ble rev2
Canbus adapter mcp2515 
Hall sensors 
Fingerprint module
Level shifter ( for canbus module 5v to work with the arduino 3.3v )
DS18B temperature sensor ( can be in transistor or normal with wires shape ) ( in my case i will use the transistor package and attach it in the cimate module of my e61 behind the fan where the original system draws air to see the cabin temp )
Mini 5v relays




Remote start Features:

Remote start car with beacon based on proximity
Remote start car with phone based on proximity ( requires app to be open )
Ability to lock,unlock the car from the app
Ability to remote start from the app
Ability to turn off the engine ( if rpm is less than 1000rpm )
Abilliy to restart the engine in case of stall ( requires clutch to be pressed )

Climate Remote start Features
Ability to set between winter or summer mode
Ability to set the temperature between 18C and 30C
Abillity to remote start for climate only with ( AC button ) ( Engine will turn off when desired temp is reached

The app can display various errors and for some even say them out loud 
Shifer not in neural
Parking brake not on
Battery low
Phone bluetooth off



