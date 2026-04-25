# SPARS

A Wifi Enabled System which helps Geriatric Patients have 24/7 Presense, Heartbeat and Breathing monitored in non-invasive way.
Our Presentation pitch can be found here -> https://drive.google.com/file/d/1QqP8J5yMbppZRnAkbPIismYOAv2ojp6g/view?usp=sharing

### Architecture

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/56cb63bc-30d2-4b4f-b3dc-3cc76a77e96f" />
<img width="989" height="590" alt="image" src="https://github.com/user-attachments/assets/0aa1c394-7a6f-41c0-9695-6ecb250e3568" />

### About 

The ESP32-S3 is really good at capturing wifi signals. It can get 64 of these signals at the time and send them to a server that is running Rust. This server then figures out how different these signals are from what it sees in an empty room.
Here is how it works:
1. The server looks at the signals. Calculates the difference in the phase of the signals. The ESP32-S3 captures wifi signals. Sends them to the server.
2. The server compares these signals to what it sees in a room. The server then uses this information to make a picture of the room. It does this by making a grid that shows where all the signals are. The server uses the wavelength of the signals to figure out how strong they are. This helps it make a detailed 3D picture of the room. The server can even track where someone is in the room. It uses an algorithm to find the center of the movement. This algorithm is really good at finding where someone is. The server then makes a heatmap that shows where the person is and how they are doing. The best part is that it does not need a camera to do this. The ESP32-. The server work together to track the persons position and vitals. They do this in time so it is really useful.


