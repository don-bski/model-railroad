### Model Railroad
**OS: Linux RPi-3**<br/>
An advanced model railroad control program written in perl. Used for automating things like block occupancy 
detection, track signaling, turnout positioning, and reverse loop polarity. Uses forked processes for signal
indications and slow motion turnout positioning using hobby servos. A perl based barebones webserver is
implemented for operational status display in computer or phone web browser.<br/>
<br/>
The Raspberry Pi 3 model B was used in this project though newer versions will also work. Off-the-shelf RPi
hardware 'hats' interface the layout sensors and turnout servos. One custom hardware hat was constructed
since no commercially available item could be found at the time. It drives the trackside semaphore signals 
using a software driven 32 bit 74HC595 shift register. Hardware schematics and layout details are included.<br/>
<br/>
While this code is specific to this model railroad layout, the design concepts and software code are
adaptable to other model railroad projects. The code also contains test functions which are useful during
construction, troubleshooting, and maintenance of the layout. 

