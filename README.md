### Model Railroad
**OS: Linux RPi-3**<br/>
This repository contains an advanced model railroad control program written in perl. Used for automating things 
like block occupancy detection, track signaling, turnout positioning, and reverse loop polarity. Uses forked 
processes for signal indications and slow motion turnout positioning. A perl based very basic webserver is 
implemented for display of operational status by computer or smartphone web browser.<br/>
<br/>
The Raspberry Pi-3 model B was used in this project. Newer versions such as the RPi-4 or RPi-5 should 
also work. The RPi uses Raspberry Pi linux which includes perl and code libraries for driving GPIO pins. 
Off the shelf RPi hardware **'hats'** interface the layout sensors and turnout SG90 micro servos. One custom 
hardware hat was constructed since no commercially available item could be found at the time. It interfaces 
the trackside semaphore signals using a software driven 32 bit shift register made up of 74HC595 ICs. Hardware 
schematics and layout details are included.<br/>
<br/>
As distributed, the above code is a snapshot of what is currently running on my layout. Place the downloaded code
in a convenient location on your RPi. Use **perl DnB.pl** at the operating system command line to run it. Use 
**cpanm** or **MCPAN** at the OS command line to install any needed perl modules. There is a **-h** option to 
display the usage text if you get that far. Study the code and internal comments to gain understanding. Then copy
and modify the parts of the code that best fit the needs of your project.<br/>
<br/>
While the code is specific to this model railroad layout, the design concepts and software are adaptable to 
other projects. The code contains test functions which are useful during project construction, troubleshooting,
and maintenance. See the browser based documentation in the **doc** folder for further details. For an operational 
perspective, see the **DnBOperatorGuild.pdf** in the **doc** folder.
