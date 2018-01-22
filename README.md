# Build Instructions on Project Teemo (Voice Recognition)

## Table of Contents
1. [Introduction using a system diagram](#introduction-using-a-system-diagram)
2. [Bill of Materials and Budget](#bill-of-materials-and-budget)
3. [Time Commitment](#time-commitment)
4. [Mechanical Assembly](#mechanical-assembly)
5. [Soldering](#soldering)
6. [Power Up](#power-up)
7. [Unit Testing](#unit-testing)
8. [Production Testing](#production-testing)
9. [Reproducible](#reproducible)

### Introduction using a system diagram

![Diagram](https://raw.githubusercontent.com/patng2007/VoiceRecognition/master/images/AWS-Overview2.png)

Welcome to Project Teemo build instruction. Project Teemo is a voice interface system that allow you to interact with Amazon AI (Alexa) to be able to complete task given through microphone input. On this page, you will find instructions on how to build Project Teemo which include how much it will cost, type of materials needed, how long it will take and etc. Following these instruction will guaranteed that your own "Alexa" system will work perfectly.  

### Bill of Materials and Budget

Total cost of this project is $138.95.

Reason why the cost is this low is because the speaker  + AUX cable is something that I had before doing the project. Below I had link the one that I was using. For the speaker, you need to spend alot of money to get an expensive one as a $30-50 one would be fine.

1. Raspberry Pi Starter Kit ($99) - <https://www.amazon.ca/CanaKit-Raspberry-Complete-Starter-Kit/dp/B01CCF6V3A/ref=sr_1_4?ie=UTF8&qid=1516583160&sr=8-4&keywords=raspberry+pi+3>

2. USB sound card ($12.99) - <https://www.amazon.ca/TROND-AC2-Microphone-Plug-N-Play-Compatible/dp/B014ANW4VU/ref=sr_1_2?ie=UTF8&qid=1516583228&sr=8-2&keywords=usb+sound+card>

3. 3.5mm Microphone ($9.99) - <https://www.amazon.ca/Neewer-3-5mm-Hands-Computer-Microphone/dp/B005DJOIHE/ref=sr_1_3?ie=UTF8&qid=1516583275&sr=8-3&keywords=3.5mm+microphone>

4. Speaker ($169.99) - <https://www.bose.ca/en_ca/products/speakers/portable_speakers/soundlink-color-bluetooth-speaker-ii/buy.html#EcommerceArea&v=soundlink_color_ii_red> 

5. 3.5mm to 3.5mm AUX cable ($6.54) - <https://www.amazon.ca/AmazonBasics-3-5mm-Stereo-Audio-Cable/dp/B00NO73MUQ/ref=sr_1_3?ie=UTF8&qid=1516583538&sr=8-3&keywords=aux+cable>


### Time Commitment

For this project, you could get this up and running in a matter of hours if you have all the parts to start building. If not, the process could take a week dues to item being delivered. If you have Amazon Prime, you could get them in like 2 days as most of these item fall us Amazon Prime shipping. Long downtime during this project is waiting on the installation of the Alexa application as it take over an hour. 

### Mechanical Assembly

1. Unbox all the parts that has arrived.
2. Take the 3.5mm microphone and connect it to the USB sound card.
3. Connect the USB sound card to one of PI USB port
4. Connect one end of AUX cable with the speaker and the other end to 3.5mm output on the PI.

[Click for the picture on how it look](https://raw.githubusercontent.com/patng2007/VoiceRecognition/master/images/IMG_0744.JPG)

### Soldering

This project doesnt require you to solder anything as all the parts are connected to the PI external ports. 

### Power Up

Before powering your PI, make sure the SD card that is included in the kit has NOOBS Operating System installed on it. To check, plug in the SD card to your computer if there are files inside then you are good to go. If you don't have it then [click here for it](https://downloads.raspberrypi.org/NOOBS_latest) and put them into the SD card. 

Once this is done, you can power up your PI and go through instruction to setup the PI.

Before you can start installing the software, you have make sure the audio output is set to 3.5mm jack which can be done by going to the top left corner of the PI UI and a dropdown menu will appear. Go down to preferences and audio device setting. Here you can change the sound card so the audio is being outputted to 3.5mm and input from the 3.5mm microphone.

### Unit Testing

[Alexa Setup Link](https://github.com/alexa/alexa-avs-sample-app/wiki/Raspberry-Pi#lets-get-started)

Follow this link as it has all the instructions to setup the software for this project. Make sure not to enable the wakeword. 

### Production Testing

Once the program has successfully ran the application, you can begin to mess around with the applcation that Amazon has created. Alot of the skills are not included in sample app so this will require you to create the skill in order to get it working (Future Project Idea).

### Reproducible 

By following these instruction given, you will be able to create your own "Alexa" system on a raspberry PI very easily as you don't have to research anything since it was given to you. I will link my Github which has documents on the project if you feel like reading them. 
[Github](https://github.com/patng2007/VoiceRecognition)
