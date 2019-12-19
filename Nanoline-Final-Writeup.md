# R2-G1 - 2013 Nanoline Competition
**Nanoline Explained**

## Final Writeup Report

[//]: # (Image References)

[image1]: https://github.com/joshrwhite/R2-G1_Nanoline-Competition-2013/blob/master/images/EngineersNotebook.PNG "EngineersNotebook"
[image2]: https://github.com/joshrwhite/R2-G1_Nanoline-Competition-2013/blob/master/images/Diagram.PNG "Diagram"

The R2-G1 robot’s electronics system is designed completely around the Nanoline system. We essentially have four peripherals that we are using to make our R2-G1: The Nanoline GSM Module, Telco Brushless motors with Double Pull Double Throw relays, light emitting diodes, and finally, an Arduino with a MP3 shield to process MP3 files and play them through speakers. 

The G.S.M. module is currently our primary method of controlling the entire system, with hopes of possible future control of motion via ultrasonic/photo eye. Essentially the G.S.M. module is receiving SMS texts as thoughts and relaying them to the Nanoline Controller, or "the brain”, which then executes the thoughts.

The motors we are using are simple brushless motors from Telco electronics, and are used with double pull, double throw, DPDT, relays which are used to control change the polarity of the input power, which changes direction of rotation on the motors, we have three motors total in the system, two to drive wheels that provide movement to the unit, and one that rotates the dome on the unit. These run on 12 volts optimally, we currently use a 9 volt power supply, in a best case scenario down the road we could get the R2-G1 to run on two 12 volt batteries in a series, with the motors power coming directly off of one batteries.

Light emitting diodes, or LEDs are used purely for aesthetic appeal. We will have them in the dome and will use two separate color LEDs: red and blue. They are mounted to the dome and the nanoline controls the blinking of them.

Finally the adruino with MP3 shield is powered by a separate battery pack, due to how small a voltage is required, only 5 volts. The adruino process the MP3 audio files, and plays them through a speaker. The nanoline controls the adruino by switching the adruino’s inputs which allows us to play specific sounds, and we also have  a 3 axis accelerometer connected to the adruino to allow audio to be played as the R2-G1 is bumped, or while moving.

### Inputs

### Outputs

The R2-G1 build is expressing five different outputs. Three of the five are motion of the bot. The Controller is positioned in the middle of the bot while the three motors stem out to the head and two legs. The fourth output is the lights in the head blinking and changing colors. The last output is that of the Arduino which was fully explained in the previous presentation. The Nanoline Controller is the source of its ability to move and make sounds as well as launch a lightsaber.

Forward motion coming from motors driving two wheels are the foundation of the “wow” factor. The Nanoline Controller, being at the center of the back panel, has outputs which will be the motors lifeline to power and command. Commands come from either text messages going through the GSM Module or controls from an auxiliary controller which will resemble the Nanoline interface. Lack of commands results in lack of motion. Without this motion, the build would simply be a prop.

Additionally, the head/dome of R2D2 swivels on an axis. That motion is the result of the last motor receiving commands via the Nanoline Controller. The head’s ability to spin is also the means by which the Lightsaber Launcher functions. Through a pulley system, connecting to the head, the lightsaber will be released. Had it just been limited to ground plane motion, a spectator would explain its motion due to remote control or “fake” motion. With the head swivel, there is a sense of autonomous control coming from the robot itself.

Light emitting diodes, or LEDs are used purely for aesthetic appeal. We will have them in the dome and will use two separate color LEDs: red and blue. They are mounted to the dome and the Nanoline controls the blinking as well as the magnitude of each color.

Our last output brings emotion to the robot. X-axis motion is eye catching, but merely eye candy, grabbing only the visual sense. The output running to the Arduino, the output that will tell the Arduino to turn on or off, is dependent upon the Controller. If the Nanoline Controller were not there, then the Arduino would be a static function that has no background story. Because we do have the Controller, the Arduino emits sound which will grab the audible sense as well. If a sense of autonomous control was not enough, then a sense of life will not only bring spectators to the edge of their seat, but will get them standing just to see how it works. 

If the Nanoline Controller were not present as the heart, allowing outputs to receive commands and activate, then the R2D2 would be an inanimate object. The R2D2 build will be able to move forward and turn via outputs running through the Controller. She will also be able to rotate her head via commands given to the Nanoline Controller. In addition to all of these actions, the bot will be able to “see” due to its LED eye and “speak” due to the Arduino emitting a sense of emotion and, ultimately, life.

### Diagrams

This drawing in our Engineer’s Notebook mimics that of the human body in a Human Anatomy textbook, showing the inside of the R2D2 build and defining how she comes to life:

![EngineersNotebook][image1]

![Diagram][image2]
