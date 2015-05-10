# KnockKnockApplication
server client application
Author: Humberto Sainz
Date 3/13/2015
-------------------------------------
EXECTUING/RUNNING
					
There are two ways to run this code.	

Running from Eclipse

Import the project root directory (KnockKnock) into Eclipse. You can then run the program from the Run menu. The 
main method is located in the KKMutliServerGUIController. 

-------------------------------------
SRC CHANGES

The source files may be found under in KnockKnock/src directory. There were several changes made to
many of the classes provided originally.

kkserver.KKMultiServer
The KKMultiServer creates a new KKMultiServerThread for each client that is created. The following changes were
made to improve OO design and functionallity:
	(1) main method removed. code found in main was moved to run() method.
	(2) added several instance variables to control when to stop creating new clients and to control
	    threads. 
	(3) added some functional methods to determine whether or not the server is running and accepting clients
	    and to stop and start the server.

kkserver.KnockKnockClient
The KnockKnockClient class is used to create a GUI interface to interact with the server. The following changes 
were made to improve the OO design and functionallity:
	(1) removed the main method. code to communicate with the server was replaced completely.
	(2) added GUI to allow for simplier interaction with the server. 
	(3) added lots of functional methods to help with apperance and processing input.

kkserver.KnockKnockProtocol
The KnockKnockProtocol is used to control how the server and client communicate with eachother. The following 
changes were made to improve the OO design and functionallity:
	(1) added JokeState enumeration to control the state of the joke (replaced int control structure)
	(2) added method to load in jokes from files (knockknockclues.txt and knockknockanswers.txt)
	(3) added code to randomize jokes upon loading files. 

-------------------------------------
DOC

The JavaDoc may be found after extracting the source files (see above for extraction).The documentation may be
found in KnockKnock/doc directory. 

 
