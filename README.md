# Analog-Clock
A simple analog clock by following the tutorial of Web Dev Simplified on YouTube
# What The Project Does
This project displays a working analog clock that shows the current time with three moving hands — hours, minutes, and seconds. The clock face shows all 12 numbers positioned in a circle, and the hands rotate smoothly in real time to reflect the correct time. It updates every second automatically.
# Tools / Languages Used

HTML — structures the clock face, the three hands, and the 12 numbers

CSS — styles the circular clock face, positions the numbers around the circle using CSS custom properties and rotation, and styles each hand with different sizes and colors

JavaScript — calculates the correct rotation angle for each hand based on the current time and updates them every second using setInterval

# Steps To Build And Run

Create three files — index.html, styles.css, and script.js

In the HTML, create a .clock div containing three hand divs and 12 number divs

In the CSS, use border-radius: 50% to make the clock circular, and use transform: rotate() with CSS custom properties (--rotation) to position each number around the face

In the JavaScript, use new Date() to get the current time, calculate each hand's rotation as a ratio of its full cycle, and apply it using style.setProperty

Open index.html in any browser to run it — no server needed

# Key Features

Smooth hand positioning — each hand's rotation is calculated as a ratio rather than fixed steps, so the minute hand moves gradually as seconds pass, and the hour hand moves gradually as minutes pass, just like a real clock

CSS custom properties for rotation — instead of hardcoding angles, the CSS uses --rotation variables that JavaScript updates dynamically

Numbers positioned with pure CSS — each number is rotated around the clock face using CSS transforms and custom rotation values, requiring no JavaScript for layout

# Challenges

Positioning the 12 numbers evenly around a circle using CSS rotation was tricky — each number's entire container div is rotated, placing the text at the correct clock position

Calculating the hour hand ratio correctly required accounting for minutes and seconds too, so the hand doesn't just jump every full hour but moves continuously
