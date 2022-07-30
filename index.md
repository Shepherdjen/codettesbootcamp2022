### 10.2 Setup Dev Environment for ESP32 S2
the first session was an online session. The teacher went over the slides and instructed the students to set up our  dev environment for the esp32 s2 using the instructions from slide 13.



After setting up the environment everyone had to test out the environment using the instruction in slide 17.


Note; i was unsuccessful in setting up my esp32 s2 environment ,so i could not do the test on day 1 of week 1.

The second session was and in lab session
With the help of one of my classmates I was able to set up my environment and do the test.
The first test was to create a Web Server (with websockets) using esp32 s2 in arduino.
How:
Step 1 was to connect a led to pin 15 of the  esp32 s2. And create a folder to save the code for the webserver. In this folder create another folder named data (the html index will be saved here.
Step 2 Install spiffs(if you don’t have it already) and the needed libraries in the Arduino IDE.
Step 3 Open a new Arduino ide sketch and paste this code

The second test was to create a web server with multiple sliders to control LED brightness. 
How:
Step 1 was to connect the leds to the  esp32 s2. 
Step 2 Install spiffs(if you don’t have it already) and the needed libraries in the Arduino IDE.
Step 3 create a folder to organize your files
          
Arduino sketch that handles the web server;
index.html: to define the content of the web page;
sytle.css: to style the web page;
script.js: to program the behavior of the web page—handle what happens when you move the slider, send, receive and interpret the messages received via WebSocket protocol.
Step 4 copy the codes from https://randomnerdtutorials.com/esp32-web-server-websocket-sliders/
Step 5 connect the esp32 s2 , upload the code and open the html file.
 Results


### MQTt and html
In this session we were introduced to mqtt lens ( A chrome plugin). The class was instructed to download the Mqtt extension and then connect to the mqttwebserver test.mosquitto.org.
After the lesson i used the link provided in the slide and went on w3school.com to learn more about HTML, Css and javascript.(i haven't learned everything yet)
We were also instructed to create a mockup of the chataplication we wanted to create and to create an html file with div and wire up the js code.
Addpicture of mockup








### webchat
In the lab session we were instructed to continue working on our web chat application. I managed to create a web interface but I could not connect to the mqtt server. 
After some time everyone changed because test.mosquitto.org was giving problems.
I still was able to connect though and decided to skip that and work on the styling for my webchat.
This what the chat looked like:


This was styled using the css tutorial on w3schools

### W3 continuing with webchat
In this session we went over how far we were with the webchat application and had to share our scenes. I still was able to connect to the mqtt server now but was not able to send message. I kept getting an error in line 1 of my html.

I tried putting the js code and my styling (css)in a different file but I still kept getting the same error
I finally discovered why I could not send messages. I made a few mistakes in the div class for the button. 
The code is supposed to look like this:
<div class="text" class="chatbox" id="chatlog">
      <input class="input"type="text" id="chatInput" id="sendMesageButton>
        <button class="sendbutton">
             <button onclick="sendMessageButton(getElementById('chatInput').value);getElementById('chatInput').value='';">Send</button>
			 </div> 
															 
But i had this instead:
															 
<div class="text" class="chatbox id=chatlog>
      <input class="inpt"type="text id="chatInput" id="sendMesageButton>
        <button class=sendbutton">
             <button onclick="sendMessageButton(getElementById('chatInput').value);getElementById('chatInput').value='';">Send</button>
			 </div> 

So after I finally got the code to work , I added more. I created another app.js file and added the new javascript there. With this javascript I was able to see who entered the chat and see the messages sent in the chat.



I also set up my Node Js environment. I had to do this twice because I didn't wait for everything to download the first time and shut down my terminal window.
So not everything was installed.
															 
### Mongodb
															 
### github
we were shown how to use github to document our work.
### 3D printing
we were instructed to dowload cura 5.0.0. . in th online session we were shown how to use it.															 
															 
															 
															 
															 




