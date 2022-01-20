# automatic-pet-feeding-system

# 1.	INTRODUCTION
                        Pets must be provided with food and water time to time , but because of the busy life we may sometimes find ourselves away from home and may not be able to feed our pet. Animal feed distribution systems are becoming very common nowadays and are used greatly both on a domestic scale as well as on a larger scale in commercial applications. Animal feed distribution systems come in many different forms with different ways to control how the feed actually gets distributed. Whether it is a manual system, an automatic system on a timer, or a sensor-based system; there are many different ways to accomplish the same end outcome, with some of the routes being more efficient than others. 
The use of sensors is a huge added benefit when it comes to feed systems because it automates the process completely, allowing for minimal human interference. Many users are looking for a system that is not only capable of running on its own, but also one that is visually appealing, whether it be a dog, cat, hamster, or any other sort of pet, these animals need to be properly cared for and nourished. Often times, a source of stress for these animals can be not getting the proper amounts of feed or not getting fed on time. This is a sad reality that leads to malnourishment and eventually abandonment of these animals. In addition, many times feed will come in an airtight bag that pet owners can forget to close up completely after feeding pets. In this project we tried to overcome some of the challenges mentioned above with help of efficient use of technology and to feed the pet time to time. 
# PROBLEM IDENTIFICATION
          Feeding the pet time to time is one of the problems that the pet lovers face because of the busy life. It may not be possible that always the feeder is present physically with the pet when the pet needs food. Our project addresses this issue. Our problem statement is to provide a means of automatic feeding to the pets by giving command over the google assistant.

# PROPOSED METHOD:
                            Here we introduce a system “automatic pet feeding system using google assistant and node MCU” which helps the feeder when he is not nearby pet. The system feeds the pet 
by receiving the instructions from the feeder given through google assistant with help of node MCU
and NTP severs.

# WORKING PROCEDURE 
1.	In this project, we are using a Node MCU ESP8266 as the main controller, a Servo motor to open and close feeding Container, a bowl to dispense the food, and a 16*2 LCD to display to see the update and time of feeding. We will get the time from NTP servers.
2.	In the feeding container food is stored by the feeder which is attached to the stand at the height of 200cm away from the dispense bowl. 
3.	When feed command is received by the NODE MCU, it activates the Servo motor which is used to close and open the feeding container to dispense the food in the bowl. 
4.	The current time and feed time will be displayed on the 16*2 LCD. 
5.	Here we use two platforms, Adafruit IO is a "open data platform that allows you to aggregate, visualize, and analyze live data on the cloud".                                              
6.	IFTTT aka ‘If This Then That’ a free web-based service to create chains of simple conditional statements, called applets to enable the google assistant. We have to create an applet in which we will integrate the Google Assistant with Adafruit IO.
7.	To feed the pet, we have to Say "Okay Google. Feed my pet" to the Google Assistant. Google Assistant will recognize the phrase and respond with "Ok Task is complete." 
8.	Node MCU automatically sends the triggers to the Servomotor which opens the lid of the food container and dispenses the food into bowl and closes the lid after a specific interval of time.
9.	We can also program the system to dispense food at a specific time using commands like “Ok Google, feed my pet at 10 am “’
