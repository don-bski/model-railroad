### Model Railroad
**OS: Linux RPi-3**<br/>
An advanced model railroad control program written in perl. Used for automating things like block occupancy 
detection, track signaling, turnout positioning, and reverse loop polarity. Uses forked processes for signal
indications and slow motion turnout positioning. A perl based barebones webserver is implemented for display
of operational status by computer or smartphone web browser.<br/>
<br/>
The Raspberry Pi-3 model B was used in this project. Newer versions such as the RPi-4 or RPi-5 should 
also work. The RPi uses Raspberry Pi linux which includes perl and code libraries for driving GPIO pins. 
Off the shelf RPi hardware **'hats'** interface the layout sensors and turnout SG90 micro servos. One custom 
hardware hat was constructed since no commercially available item could be found at the time. It interfaces 
the trackside semaphore signals using a software driven 32 bit 74HC595 shift register. Hardware schematics 
and layout details are included.<br/>
<br/>
While the code is specific to this model railroad layout, the design concepts and software are adaptable to 
other projects. The code contains test functions which are useful during project construction, troubleshooting,
and maintenance. See the program code comments and browser based documentation in the **doc** folder 
for further details. For an operational perspective, see the **DnBOperatorGuild.pdf** in the **doc** folder.
