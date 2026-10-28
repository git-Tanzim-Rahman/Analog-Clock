# Analog Clock
A simple analog clock by following the tutorial of Web Dev Simplified on YouTube
# What The Project Does
The clock shows the current time similar to a physical analog clock using hours, minutes and seconds. The clock hands move smoothly and is updated automatically every second to show the correct time.
# Languages used:

To structure the clock face, the three hands, and the 12 numbers I have used HTNL.

CSS is used to design the circular clock face, using its custom properties and rotation I position the numbers around the circle and style each hand with different sizes and colors.

JavaScript was then used which calculates the correct rotation angle for each hand based on the current time and updates them every second using setInterval.

# How to build and run on your setup:

Open VS code and create 3 files called: index.html, styles.css and script.js

In the html file, create a .clock div containing three hand divs and 12 number divs.

In the CSS file, use border radius 50% to make the clock circular, and use transform rotate() with CSS custom properties to position each number around the clock face.

In the JavaScript file, use new Date() to get the current time, calculate each hand's rotation as a ratio of its full cycle, and apply it using style.setProperty.

Open the html file in any browser to run, no server required.

# Key Features

The hands are designed to move smoothly. To achieve this each hand's rotation is calculated as a ratio rather than fixed steps, so the minute hand moves gradually as seconds pass, and the hour hand moves gradually as minutes pass, just like a real clock would.

The numbers are positioned with CSS only and its done by rotating each number around the clock using CSS transform and custom rotation values therefore no JavaScript is used for layout.

# Challenges

I had very little prior knowledge about JavaScript before doing this project so it was definitely a learning moment. Other than that the project was not too difficult as I did have a tutorial to follow along to.
