# DTWSpells-DeMay

The goal of this project was to create a magic wand that is capable of recognizing distinct gestures in order to cast spells.

Once I came across a suitable stick outside I taped up the handle and made a small cardboard mechanism to help attach the microbit to the tip of it. From there I connected the microbit to my computer using a 6 ft micro USB cable which allowed me to feed the x, y, and z values of the microbit into a python script. The python script then takes this data and sends it to Wekinator via OSC messages, and as an output I set up a text and sound trigger that outputs different tones and messages for different specific gestures. This was accomplished with dynamic time warping as my algorithm and seemed to work quite nicely.

After experimenting with different gestures I quickly learned that incorporating a tilting motion seemed to highly increase the accuracy of correctly classifying the motion. With this knowledge I gave both of my spells a little bit of tilt when training the models and by the end of the process I could cast the spells I wanted to with minimal to no error. Others might be able to improve this design by using a wider variety of an increased number of gestures and finding characteristics other than tilt that will help improve the accuracy. Adding more training examples would most likely increase the efficiency of this project as well, although it may increase the computation time.

Demo video: https://www.youtube.com/watch?v=HdANo-QrEiY&feature=youtu.be

To use this set up:


