# TFTP-Using-UDP
Trivial File Transfer Protocol Using User Datagram Protocol 

## Introduction
This project was a course project for my Computer Networking course. The goal of this project was to create a GUI based file transfer system using two given classes, the UDPSender and UDPReceiver. The project required me to edit the two given classes as needed and create a GUI for the user to use to send and receive messages. The program must also save the sent and received messages to a respective file.

### Classes

* **UDP Receiver** - one of the given classes edited to run as a Thread. This class enables a machine to receive messages from another machine, and writes the received message to both the GUI and a text file.
* **UDP Sender** - one fo the given classes edited to run as a Thread. This class enables a machine to send messages to another machine. It sends the message to the specified IP address, and writes the sent message to a text file.
* **Text Interface** - this class creates the GUI interface. When the "Send" button is pressed, it creates a new thread for both sending and receiving, and runs the threads.

## Instructions
* To send a message:
  * Type the desired message into the "Message" box.
  * Enter the receiving IP address into the "Send to" box.
    * *If no IP address is entered, it automatically sends the message to the localhost.*
  * Click "Send".
* Received messages automatically appear in the "Incoming Message" box, with the sending IP address appearing in the "Sent from" box.

![alt text] (https://github.com/nikkipruitt182/TFTP-Using-UDP/blob/master/ReadMe%20Images/GUIInterface.png "User Interface")

## Samples
* Send a message without an IP address.
![alt text] (https://github.com/nikkipruitt182/TFTP-Using-UDP/blob/master/ReadMe%20Images/MessageSentToLocal.png "Send a message to the default receiver")
  * The sent message file:
![alt text] (https://github.com/nikkipruitt182/TFTP-Using-UDP/blob/master/ReadMe%20Images/DefaultSentMessageFile.png "Sent Message File 1")
  * The received message file:
![alt text] (https://github.com/nikkipruitt182/TFTP-Using-UDP/blob/master/ReadMe%20Images/DefaultReceivedMessageFile.png "Received Message File 1")

## Note
Due to a misunderstanding of the instructions, this program does not actually transfer the files. However, it does send a message to another machine using UDP, making it behave more like a person-to-person chat room. (*Adding the code to work with file transfer may be a project for another day.*)