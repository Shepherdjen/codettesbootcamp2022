# chat
## 10.2 Setup Dev Environment for ESP32 S2
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


## MQTt and html
In this session we were introduced to mqtt lens ( A chrome plugin). The class was instructed to download the Mqtt extension and then connect to the mqttwebserver test.mosquitto.org.
After the lesson i used the link provided in the slide and went on w3school.com to learn more about HTML, Css and javascript.(i haven't learned everything yet)
We were also instructed to create a mockup of the chataplication we wanted to create and to create an html file with div and wire up the js code.
Addpicture of mockup








## webchat
In the lab session we were instructed to continue working on our web chat application. I managed to create a web interface but I could not connect to the mqtt server. 
After some time everyone changed because test.mosquitto.org was giving problems.
I still was able to connect though and decided to skip that and work on the styling for my webchat.
This what the chat looked like:


This was styled using the css tutorial on w3schools

## W3 continuing with webchat
In this session we went over how far we were with the webchat application and had to share our scenes. I still was able to connect to the mqtt server now but was not able to send message. I kept getting an error in line 1 of my html.

I tried putting the js code and my styling (css)in a different file but I still kept getting the same error
I finally discovered why I could not send messages. I made a few mistakes in the div class for the button. 

The code is supposed to look like this:															 
<div class="text" class="chatbox id=chatlog>
      <input class="inpt"type="text id="chatInput" id="sendMesageButton>
        <button class=sendbutton">
             <button onclick="sendMessageButton(getElementById('chatInput').value);getElementById('chatInput').value='';">Send</button>
			 </div> 
So after I finally got the code to work , I added more. I created another app.js file and added the new javascript there. With this javascript I was able to see who entered the chat and see the messages sent in the chat.



I also set up my Node Js environment. I had to do this twice because I didn't wait for everything to download the first time and shut down my terminal window.
So not everything was installed.
															 
## Mongodb
															 
## github
we were shown how to use github to document our work.
## 3D printing
we were instructed to dowload cura 5.0.0. . in th online session we were shown how to use it.															 
															 
															 
## canvanizer
i created a account on canvanizer to creat a canvas.

# Business model canvas

## 3.1 What is a business model canvas?
A business model canvas(a one sheet business plan) is a visual representation of a business model, highlighting all key strategic factors. So a business model canvas basically gives you an overview of the company's workings, customers, revenue streams etc.
Business model canvases are most used by start-ups but it is also used to document existing company’s. 
Alexander Oswalder was the first person to propose the use of a business model canvas. 
Before making a business model canvas you have to have a business plan (Plan for successful operation of a business or startup that identifies Sources of Revenue and Target Customer Base combined with details of Financing), only then can you start making a canvas.
## 3.2 the building blocks
When making a Business model canvas you have 9 essential building blocks.
Those building blocks are :
Key partners: who will be your key partner/suppliers? Which key resources do they provide?

Key activities :what are the key processes and task we need to create our value proposition?

Key resources: what key resources do our key activities require?

Value proposition: Which of our customers problems are we helping to solve?Value proposition look like?

Customer relationships:what type of relationship do you want with customers?Which fits best with each segments?

Channels:To which channels do each of our segments want to be reached?Which ones are most cost efficient?

Customer segments :For whom are we creating value?Who are the most important customers.?

cost structure: I mean and elements of operational expense? (Floating variable cost,inventory ,WIP and capital assets).
Revenue streams: From which channels and segments? how much does each contribute to overall revenue?

![image1](https://user-images.githubusercontent.com/109770876/182912849-82dbe578-8439-4462-b3e7-43eaf7d78452.png)



## 3.3 Why use BMC?
A few resons to use a BMC are because it describe your business in page, it si costumer focused,its easy to present, Easy to benchmark peers/competitors etc.
## 3.4 my BMC
Before making my Bmc i had to research about my product, what is needed to make it , the development process, what kind of value it will bring to customers' lives and how I will finance building the product.
https://next.canvanizer.com/canvas/r0C4ZGpeowqQX
![image2](https://user-images.githubusercontent.com/109770876/182912930-64c1f3c5-bef6-4247-a3d6-14a53c6e601d.png)



## 3.5 my poster
![image3](https://user-images.githubusercontent.com/109770876/182912961-a8c5db3f-0832-4c36-8dfb-a42cd6635b2a.png)
# 3D Printing
## 7.1 What is 3d printing?
3D printing is the act of adding layers and layers of filament (thermoplastic feedstock for fused deposition modeling 3D printers) to create a solid object using a 3d printer. 3D printing is an additive process because you are adding layers to create an object. 
## 7.2 type of filament?
Filament is the thermoplastic feedstock for deposition modeling 3d printers. There are many different types of filament but in the lab i will be working with the PLA (polylactic acid filament ) and the ABS( acrylonitrile butadiene styrene filament).
![image14](https://user-images.githubusercontent.com/109770876/182914823-e14a635a-bddb-4b92-8f57-5a7b281bfcd3.png)

Although both filaments are thermoplastic, The PLA is organic , stronger and stiffer than the ABS but the PLA has a big disadvantage because it does not have very good heat resistant properties because of this PLA is more of a hobbyist material. ABS on the other hand is weaker and less rigid than than the PLA  but it's also tougher and lighter than the PLA. That is why ABS is the preferred filament when making prototypes.
## 7.3 printers
There are two printers in the lab, the anycubic 4 max pro and the anycubic predator(deltabot).
The anycubic 4 max pro has an enclosed printing space with a large build volume to enhance printing quality. It is also out of box and there is no need to assemble. It is also safe for children because it has an optional auto power off feature. There is also a sensor that turns off the machine when it runs out of filament.
![image9](https://user-images.githubusercontent.com/109770876/182915001-d7c15b58-5e6f-441c-9534-e1c8a4d827d3.png)

The anycubic predator is a bit more for advanced 3d printing. It uses delta bot ( 3 robotic hands attached to the printhead to deposit material. This is the printer that I will be using in this bootcamp.
![image2](https://user-images.githubusercontent.com/109770876/182915021-4eb5a29e-2ba8-4064-830a-f04c7115fa27.png)

## 7.4 printing software Cura 5.0.0.
For the boot camp i will be using Cura 5.0.0. I prefer to use this version because 1. It is the latest version and 2. Its is easier to use because of it has different profiles with preset parameters( this was not available in the older versions.)
I downloaded Cura from this link :https://www.windowsinside.com/software/ultimaker-cura/download this version can be used on a laptop with 32 bit and 64 bit.
![image8](https://user-images.githubusercontent.com/109770876/182915041-5d4d30c2-143d-4a63-9c04-6ee5325d603f.png)


## 7.5 Basic PLA parameters
There are some basic parameters you should/ pay attention to when 3D printing. What you need to pay attention to is the : Quality, speed and temperature, filament, fill , support and machine.
Quality: there are 3 important things to pay attention to by quality. The layer height(the height that each printed layer will have), shell thickness(the thickens of the other shell of what you are printing) and enable retraction(retraction has to be enabled or else the filament will leak when the nozzle is moving from point a to point b)
Speed and temperature: the3 important things to pay attention here to are the: print speed mm/%(the speed at which the machine prints),printing temp(the temp at which the filament will become liquid), bed temperature( the bed that will be used to print also need to be hot(so the temp of the plate)).
Filament: here there are two things to pay attention too. 1. The diameter: this depends completely on the size of the filament you are using and nozzle size for example the PLA filament is 1.75 mm. So for the the diameter i will put 1.75 mm. 2.  The second thing to pay attention too is the flow:
Fill : Here you need to pay attention 1. the bottom/ top thickness: this like the shell thickness 2.full density:  this is to determine how solid you want your object to be. The higher the density the more solid your object will be .
Also the higher the density the longer it will take to print.
Support: here you pay attention to support type: this has to be enabled so your 3D print will be supported or else it will collapse. Platform adh type: this is so the machine print a parameter around your 3D before it start on your design so the filament can start running.
Machine: pay attention to the nozzle size.

Some basic diameters for PLA:(change to suit your needs)

quality
Layer height(mm)
0.2
Shell thickness(mm)
1.21
Enable retraction
on


Speed and temperature
Print speed(mm/s)
50
Print temp(c)
195
Bed temp(c)
65


Filament
diameter(mm)
1.75
flow(%)
100


Fill 
Bottom/top thickness(mm)
1.2
Fill density(%)
25


Support type
Support type
Everywhere 
Platform adh. type
Brim



Machine
Nozzle size(mm)
0.4


## 7.6 Setting up Cura and Using it.
After installing Cura I needed to set it up so I could use it. This was easy because as stated in 7.4 This version of cura already has a lot of presets.
First thing you need to do after installing cura is adding a printer. This is done by going to settings, the add printer ,then add a non network printer and then selecting the printer you will be using. I am using anycubic predator so i had to scroll down to anycubic and selected anycubic predator.

settings:
![image1](https://user-images.githubusercontent.com/109770876/182915380-ccad81a8-734b-482b-b1d9-97ce4264eae6.png)
![image11](https://user-images.githubusercontent.com/109770876/182915595-3253fddf-0ad0-48be-9a18-0838b77da5c8.png)

Printer:
![image3](https://user-images.githubusercontent.com/109770876/182915524-42b22239-ed62-4cb3-98d9-be476e210f28.png)


Press on add a non-networked printer:
![image10](https://user-images.githubusercontent.com/109770876/182915852-fbc1184a-e591-474f-bb9d-ecfef37340e7.png)

Select printer you will be using:
![image13](https://user-images.githubusercontent.com/109770876/182916009-df26687c-bd58-44e1-8f91-2869e2734ba7.png)


### 7.6.1 checking printers
After adding a printer you can go back to check and see if its has been added by going back to setting and hovering over  printer. The printer that you have added should show up there.
For example:
![image3](https://user-images.githubusercontent.com/109770876/182916452-9b30a0e8-675b-4603-8432-449f0f6e6f7a.png)

Since i only have anycubic added for now that is the only one that has shown up, but if you have more printers added they will show up.
### 7.6.2 deleting printers
Now if you have a printer added but want to remove it. That is very simple to do.
Simply go back to setting then printers and select manage printers. In manage printer select the printer you want to delete and then click on the right options list and press remove.

![image4](https://user-images.githubusercontent.com/109770876/182916638-4c183a6e-7d32-41c5-8415-ec626e26af58.png)

![image5](https://user-images.githubusercontent.com/109770876/182916761-05153a7b-0175-46bb-a5ad-9e0eef10f04f.png)





### 7.6.3 checking the dimensions
After selecting the motor. If you want to check and see if the dimensions re right for your printer you go to manage printers , select the printer you want and then select mange settings. If the dimension are off then you can edit it to make it right.
![image6](https://user-images.githubusercontent.com/109770876/182918511-0f11c410-f22d-4b08-b012-bc74b19c7d5f.png)



 It is important to know the size of your printer because if you put the wrong dimension in. when the machine will try to print the nozzle might come down too hard and brake dust ruining your machine.
### 7.6.4 checking parameters
In older versions of cura the parameters needed to be added manually but in the version i'm using there are profiles with preset parameters.
To see these parameters you have to click on the top right corner menu item and then you will see these parameters.
![image12](https://user-images.githubusercontent.com/109770876/182918602-4726a684-b62f-4d38-a6fe-ad8f2ed060d0.png)

Note : fill patern is the patern of the mesh stuff that is always ther when you print.
### 7.6.5 importing STL file to print.
To print you need and Stl file. An STL file is basically a file with you’re 3d design on it. The steps to adding an stl file to cura are 1.go to file on cura and click add file. 2 Select Stl file and click on open.


Note :when printing make sure your object always lays flat because if it doesnt lay flat, it will most likely collapse. Cura has an option in the side bar that lays the object flat for yoy when you select it.
Note 2:after tselctig lay flat in the side you will see a notification pop up on th botoom tight side of your screen showing you how much time your object will take to print

### 7.6.6 generating Gcode.
When you’re done adding an STL and setting up your parameters and dimensions, you need to save your object design. This is done by clicking save and saving the file with .gcode.
Gcode is…………..
After saving the file with .gcode you have to copy it to an sd card and then put that into the printer and your object will start printing.


                     # Freecad 
![image46](https://user-images.githubusercontent.com/109770876/189416257-d1a07447-f1ea-4e55-8699-1b5a6a0c62c4.png)

What is freecad?
FreeCAD is a general-purpose parametric 3D computer-aided design modeler and a building information modeling software application with finite element method support.
![image46](https://user-images.githubusercontent.com/109770876/189416257-d1a07447-f1ea-4e55-8699-1b5a6a0c62c4.png)

##How to use freecad?
##1.1 making objects with pockets.
The first thing to do is open freecad and select create  new.
![image3](https://user-images.githubusercontent.com/109770876/189416548-93594046-e728-4e16-8ec2-224896e8f780.png)

After selecting create  new this screen will appear.

![image25](https://user-images.githubusercontent.com/109770876/189416774-a78f798c-6c62-46f9-b2f4-f78f136b23a2.png)

At the top of the screen you will start. Select on that an a whole list of options will appear.
image
You have to select part design. After selecting part design this screen will appear.

![image5](https://user-images.githubusercontent.com/109770876/189416918-4f8bed31-9be8-439d-a40e-9d0e1e28cb78.png)

When the screen appears you have to look for a sketch and select that. 
After selecting create sketch some things will appear in the combo view.
There you have to select the base planes you want to work on. (i always pick xy plane).

![image28](https://user-images.githubusercontent.com/109770876/189417238-e5e48c90-ff25-4251-bcaa-2c0566172b45.png)


After selcting your base pane and selcting ok. This will appear.

![image16](https://user-images.githubusercontent.com/109770876/189417474-b1afbbe0-b42b-4d67-a0ef-404582d30e1e.png)

You then have to select the shape you want to create.

![image61](https://user-images.githubusercontent.com/109770876/189417597-6291bbfd-3cc1-4e7f-997b-4aeb22dd1692.png)


After adding you shape you to combo view and select close. 

![image37](https://user-images.githubusercontent.com/109770876/189417767-3dbc57af-81f1-457d-befc-515322dc9655.png)


After doing that you have to pick pad and your shape will created.

![image43](https://user-images.githubusercontent.com/109770876/189417996-78eac192-c914-4cc7-b173-0eb81ecac020.png)


If you want to add shapes or holesor pockets to your object. You can select the top of your object and then go to create a sketch. 
![image58](https://user-images.githubusercontent.com/109770876/189418079-5f63778e-abd1-48b2-ad16-5595803c1c73.png)

![image17](https://user-images.githubusercontent.com/109770876/189418175-d9a93797-7b76-44ce-a601-12c92b47ab27.png)


The the selcted part of your object will appear.
![image34](https://user-images.githubusercontent.com/109770876/189418379-4f2a7261-f35e-4507-a80c-0dbc6d58ee5f.png)

There you can add a shape on top and then select close.
![image33](https://user-images.githubusercontent.com/109770876/189418470-4e520c62-0085-4e04-8877-08daef0df639.png)

After selecting close , instead of clicking on pad you have to select on pocket or whole.
![image12](https://user-images.githubusercontent.com/109770876/189418592-dd245cca-f10a-430c-83dc-94aa43ad0047.png)
This will be the end result.

##1.2 freecad for cnc
1.2.1 making and object.
The first thing to do when using free cad for cnc is to make a 2D object.
![image1](https://user-images.githubusercontent.com/109770876/189418776-fdee4f56-34f9-404b-afda-2003dd3e7c59.png)

After making the 2D object you have to change your units to metric small parts (this is mandatory when planning to use the cnc machine.
You do this by going to edit then preferences.
![image6](https://user-images.githubusercontent.com/109770876/189418918-99f3d875-9a10-4c8d-af1b-5cac2026e159.png)
Then you select units.
![image56](https://user-images.githubusercontent.com/109770876/189419067-e34f4524-d846-4601-9f02-179282160803.png)


Then units system and change it to metric small parts.
![image38](https://user-images.githubusercontent.com/109770876/189419229-66807730-9e85-4cf3-b46e-2e814e3974eb.png)

After doing that select pad to make your 2D object 3D.
![image44](https://user-images.githubusercontent.com/109770876/189419353-dad0e125-7000-4f82-b116-c3ad7bb9d6d3.png)

when you make your object. Always remember to write down your debt because. It will important later on.

Object from another angel:
![image22](https://user-images.githubusercontent.com/109770876/189419457-021d9d8c-4026-471e-9e24-21ab9efacbbf.png)

Now if you want to add a pocket to your 3d design you can use the steps in 1.1 making objects with pockets. 

object with a pocket:
![image40](https://user-images.githubusercontent.com/109770876/189419572-256adb5a-9125-4147-873e-a0389003d5af.png)


##1.2.2 making jobs

The next step to making an object to cnc is making a job. To that we have to select a new workspace called path.
![image49](https://user-images.githubusercontent.com/109770876/189419763-209499fc-21b2-409c-895f-e58df0539abb.png)
next you have to select job, so you will be able to make operations.
![image4](https://user-images.githubusercontent.com/109770876/189420001-a9dd5344-85b1-4cc4-a02f-513ac5dcb0c3.png)

After selecting job this will pop up.
![image27](https://user-images.githubusercontent.com/109770876/189420266-c068dc2d-e70a-4d7c-89fb-23b181d617bf.png)

When you see this , you have to make sure body is selecting and then click okay.

Once you do that. This promp will open up.
![image10](https://user-images.githubusercontent.com/109770876/189420523-38608f5f-4b5e-4329-b1c4-0f452f84c5c3.png)

The x,y,z stand for the length, height and width of the stock you will be using to cut out your object. To make sure that the object is cut out right, the stick has to be somewhat bigger than the object.
![image41](https://user-images.githubusercontent.com/109770876/189420737-4bdbac91-71bd-443a-bed5-be6e8ed3a880.png)

As you can see I changed the x, y and z and the stock around my object got bigger.

Next thing to do is click on output. 
![image48](https://user-images.githubusercontent.com/109770876/189421043-fabcdf7d-45d0-4cd2-b2dc-c0fd8e36ef9a.png)


and this will popup:
![image20](https://user-images.githubusercontent.com/109770876/189421240-789bbc8b-75e0-4fc7-873c-4ab3d37b07bd.png)


Next you want to change the processor to ucnc.
![image15](https://user-images.githubusercontent.com/109770876/189421287-9d5d1408-ab47-41bd-91dd-c205248fbdf9.png)

then select this and save the file where you want.
![image29](https://user-images.githubusercontent.com/109770876/189421483-dda81794-038f-4ceb-a437-ce59435fdd87.png)


Note that when saving you have to save it as, UCNC OR NC.


Next step is to  go back to  setup and change origin position. To that you have to zoom in on the point you want to start cnc on and select. Then in the promp scroll down and click set origin.

![image57](https://user-images.githubusercontent.com/109770876/189421569-00c45442-b472-461f-8046-e451cebfba07.png)
![image7](https://user-images.githubusercontent.com/109770876/189421672-f4861021-9407-437d-a961-cb474ce81c89.png)
 This will be the result.
 
![image19](https://user-images.githubusercontent.com/109770876/189421789-27c252af-7d07-4d33-ba47-2678135fbedb.png)

 Then now you can click on okay.

Next is to hide the body.
![image2](https://user-images.githubusercontent.com/109770876/189421881-0d1b1e74-8399-4ac4-9d99-0199aa26f58e.png)


If you look here you can see that we have two bodies. The normal body and the model body.
You want to work with the model body and hide the normal body. To do that simply select the body and press space. You will see the body disappear and to show the model body simply select it and then spacebar and the model body will appear.
Everything should look like this when you’re done:
![image11](https://user-images.githubusercontent.com/109770876/189422061-86fd1922-819f-46b3-9c20-46452006ce70.png)


##1.2.3 making tools
We need to make tools for our cnc machine. The first is to go to tool bit doc and select.
![image32](https://user-images.githubusercontent.com/109770876/189422240-f4c1f501-4a9a-42ba-8f0a-6184e5d463a9.png)

this will pop up after selecting.
![image30](https://user-images.githubusercontent.com/109770876/189422400-b1eb017b-9e78-47eb-ae10-819aa5d94145.png)


And you will see the tools. initial y freecad does not have a 3 mm toot so you will have to create one.
To do that you have to select this:
![image51](https://user-images.githubusercontent.com/109770876/189422486-278b18f8-99bf-4886-a487-c23c47bf59d9.png)


Then this will pop up.
then select on create toolbit.
This will pop up:
![image59](https://user-images.githubusercontent.com/109770876/189423113-72b6ff6b-ee0a-4fc5-8e0d-540f757f068d.png)
you have to select endmill in this  case.
Then this will pop up.
![image31](https://user-images.githubusercontent.com/109770876/189423212-5612506b-1142-496c-bd4f-3a9a6f6ad2a4.png)


Here you then save the mill as 3mm_Endmill.fctb
 Not that you have created your mill you go back to this.
 ![image51](https://user-images.githubusercontent.com/109770876/189422486-278b18f8-99bf-4886-a487-c23c47bf59d9.png)
and your tool will be shown.

If you dubbel click on your mill. The parameter will pop up. Depending on your measurements of your mill you can change the parameters.
For example:
This the default parameters i got for  my mill:
![image60](https://user-images.githubusercontent.com/109770876/189423586-326791bd-9ba2-4eeb-972e-326534b54635.png)


but after getting the measurements for the mill i will be using in the lab i had the change the perameters to:
![image55](https://user-images.githubusercontent.com/109770876/189423624-4f786642-db5c-498d-a642-0b0f1b9a2f0b.png)
Then click okay and close it.
Next is adding the end mill to tools.
To do that you have to select tools.
![image24](https://user-images.githubusercontent.com/109770876/189423904-4889ab13-bc88-4bcd-8ed4-157f5eb60dbd.png)


And dubbel click on the endmill.
A![image26](https://user-images.githubusercontent.com/109770876/189423999-0bf25d45-ef4a-4376-9f0f-82be84e51e92.png)
And the mill will appear here.
![image53](https://user-images.githubusercontent.com/109770876/189424179-852c1909-be4e-49c3-8449-1311709dee6a.png)

Then you can delete the default tool.

![image35](https://user-images.githubusercontent.com/109770876/189424366-8b571e48-a4c9-47ea-9268-ab2cd67bfdb2.png)


Next is putting in some parameters for the 3mm endmill
You need the dubbel the endmill in tools. And this will pop up.
![image35](https://user-images.githubusercontent.com/109770876/189424381-e56f69a6-3f37-4cdd-bd03-e1ca12e64e71.png)
![image50](https://user-images.githubusercontent.com/109770876/189424524-73e4cf40-ea72-463f-ae26-09522e1117de.png)


 Now to set these parameters you will need to fiddle around with the cnc machine.
But i was given the parameters so i did not have to do that.
![image42](https://user-images.githubusercontent.com/109770876/189424663-0ce2242b-47e5-4a13-a1a8-9e57c5278c19.png)


I entered these parameters and then the mill was ready and setup.
##1.2.4 Making operations to use the tools.(profiles)
The first is to click on job and then pocket shape ( to mil out the pocket).
![image21](https://user-images.githubusercontent.com/109770876/189424790-d723d5af-8b8c-46f5-83ec-1e5431579547.png)


Then open base geometry. Is basically you select the pocket you want to work with.
To that you have selct the pocket rim you want o work with and then click add.
![image8](https://user-images.githubusercontent.com/109770876/189424867-28912300-8a36-4106-80f2-c6861ed840e1.png)
![image18](https://user-images.githubusercontent.com/109770876/189424918-dcf2c1e1-d863-4c6d-8b3d-9d2a3a5387ee.png)


When you this Then you know the pocket has been added successfully.
![image39](https://user-images.githubusercontent.com/109770876/189425145-79ff26fe-5311-4b7a-8a30-44282649c518.png)

 Next go to operation.
Edit it to look like this.
![image9](https://user-images.githubusercontent.com/109770876/189425274-eeab55f0-b027-442c-8222-3416dd52ff55.png)

Next go depths. And edit it to look like this depending on your tools and machine.
![image52](https://user-images.githubusercontent.com/109770876/189425367-4616f494-8770-47f0-b992-f349491b8152.png)

This what your depths should look like if you are milling a whole. The final always need to more than your object thickness.
 Do the same for all the other pockets and wholes. With pockets the final depths depends on how deep you wan the pocket to be.
 If  you want to sumilate the cutout. Simply click on cam simulator.
 ![image54](https://user-images.githubusercontent.com/109770876/189425491-33d30c54-252c-4537-937d-9f956f242191.png)
![image45](https://user-images.githubusercontent.com/109770876/189425527-11229342-77ce-4436-9677-d208e6e26d1b.png)


 next is to cut out base material ( so the whole thing)
First you need to make new profile and select the face and add in base geometry.
![image23](https://user-images.githubusercontent.com/109770876/189425594-db025f32-0d49-4e3e-b308-22d369193572.png)


Next the  depths and operation.
##1.2.5 adding tabs
Tabs are added to prifle that are being cutout completely.
How select the profile, option and then selct the tabs you want to use.

![image13](https://user-images.githubusercontent.com/109770876/189425729-a40f5a18-d711-4b38-b574-b53c0e2a4a04.png)
![image36](https://user-images.githubusercontent.com/109770876/189425851-02589b96-e6e0-405f-a579-9cb639632cac.png)

 ![image14](https://user-images.githubusercontent.com/109770876/189425935-3495821b-eb3d-4d58-a59d-55b92bb606a3.png)


 And then click apply.
 




														 




