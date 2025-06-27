---
title: BirdBox
author: Rehan Shaik
description: I am creating a bird house with weather/bird tracking instruments!
created_at: 2024-06-18
---

# June 20: Brain stormed on final ideas!

I wanted to do this project for a while! A bird house with weather tracking instraments but I didnt really have a clear picture on what or how to do it. I honestly still dont. But I do have a general idea on what I want this project to have. At the biggening I planned on having the rpi computer in the bird house to transmit data and video to another rpi that would up load it to a website using the wifi or display it on a screen at home. But thinking deeper into that I felt that would become very complicated for my very biggener set of knowledge. So I finallized on having the rpi collect data locally and store it on a usb where then I could take that data whenever I want to! This would still be hard for me but wayy easier then what I originally had in mind. 

I settled on having 4 sensors:
* DH22 for temp & Humidity
* BH1750 for light
* BMP280 for pressure
* Mayyyyybeeee a UV sensor if I could Find one

* rpi camera with a motion ditector to record moments in the birdhouse if a bird ever decides to move in

This project is honestly pretty big for me and have no idea on how to code all that but I have this vision Id like to give a shot at! 

I looked at some birdhouses of which I might buy so I can put the instrument mount in!

![image](https://github.com/user-attachments/assets/871b17a3-a691-4575-b2a3-0d96dd2ad6c8)
I decided to go with a birdhouse somthing like this where the instruments can sit inside under roof with a nice slant area for solar panels! Thi gave me some cad Ideas for when I move on to that faze.

[Time spent this session: 45mins]

# June 22: Worked on the theoretical code!

The plan is to collect the data locally on a USB, where I could easily remove it and look at the video and data logs. So I tried to use .CSV to store the data from the sensors for easy graphing. I strugged with this part for soo long! I spent 2 days trying to find documentation for the sensors and the file system trying to figure out how to put all of it together. The sensors so far that I decided to use after my research were the DHT22 for temp & humidity, BH1750 for light intensity and a pressure sensor BMP280. I later found out that there is a BME280 that combines temp, humidity and pressure all in one but I had already written a bit of code for the DHT22. I might change it later on. 

After searching for 2 days I swear there was no documentation on the BH1750 in micropython!! but I did find a lot of helpful ones for the DHT22 like this one: https://docs.micropython.org/en/latest/esp8266/tutorial/dht.html 

After a lot of struggling I put togehter some sort of code that I am skeptical it might work but this is just theoretical so I will deffenetly be changing it later if and when I get my parts. But fornow I finsished some stuff on the DHT22 and BH1750. The rest, like the camera and the pressure sensors, I will leave for now.

Tomorrow I want to start working on CAD!

main.py:
![image](https://github.com/user-attachments/assets/2dee60a6-16f1-4e6f-84a9-f316bfbaf6df)

sensors.py:
![image](https://github.com/user-attachments/assets/b4473ad0-1add-4142-808a-b44f04c45638)

[Time spent this session: 4hrs]

# June 27: Started on CADing!

I finally got some experience from my previous highway project in building a hackpad!. But I still wasnt the best so this casing had to be the the simplest case design. I started off by finding a birdhouse that I would buy so I can build the case off it so I started looking at amazon. All the houses on amazon were pretty tiny and was deffenetly not able to fit the whole thing in there. The case would have taken up half the space! So I switched up the game plan and decided to mount the case on the outside of the bird house and poke a camera through. I eventually found a bird house with a vent hole cut on the side where it would be perfect to slide the camera in along with a motion sensor. I just had to make sure that it was well coverd by some sort of covering from the case all the way into the bird house itself. 

The hole on the top righthand side of the bird house is where I plan to feed the camera through.
![image](https://github.com/user-attachments/assets/0a75943c-985e-42c8-9fa7-8ded8c84a578)

Now that I had the planing done on how the bird house would be mounted I started a it on the cad. I made the inside of the box 101.6mm x 101.6mm with a wall thinkness extending out 6.15mm. on the front side I cut out a whole where the camera ribon with slide through. I need to make sure that when Acually building This I add somesort of water proof cover. Along with the whole I also added 4 pegs so the rpi would sit still. To the right of the rpi I plan to on putting the sensors. It would be relativly safe here!

![image](https://github.com/user-attachments/assets/46749f5f-010a-4549-8a7d-20de301992f7)

[Time spent this session: 2hrs]




