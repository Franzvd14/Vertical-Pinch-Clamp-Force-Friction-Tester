# Vertical-Pinch-Clamp-Force-Friction-Tester
Intro: Developed a calibration procedure and Standard Operating Procedure (SOP) for a vertical pinch clamp friction tester, including custom tooling design, to ensure repeatable and accurate test results. The tester presented many hardware and setup challenges, which are discusesd below in greater detail.

Project Scope: My former employer was requesting the team to integrate and refurbish a vertical pinch clamp force tester used to measure a medical device's coating performance. Upon recieving the vertical friction tester it was not functioning properly and had significant software issues. The software issues stemmed from the use of an outdated floppy disk. Furthermore, the performance of the friction tester had to be calibrated. Due to the sophistation of the machine, a calibration protocal had to be made to calibrate the movement of the tester in the vertical direction, the movement of the pinch clamp force in the horizontal direction, and most importantly the friction force sensor in the vertical direction. 


Project Info: Due to the machine being older, it's operating system was stored on a floppy disk and which prevented the tester from starting up. To resolve this, the program from the floppy disk was successfully extracted to a USB drive. From here the windows operating system was changed, so that the startup command initiated the friction tester software directly from the USB, bypassing the use for the outdated floppy disk. The picture below shows the BIOS information screen, where the machine was changed from it's "first boot drive" from floppy disk to USB Drive.

[Testing BIOS Screen](https://github.com/Franzvd14/Vertical-Pinch-Clamp-Force-Friction-Tester/blob/main/IMG_6392.jpg)

Project Info: After successfully solving the software system issue, the user interface and testing software could now be accessed. From here, the calibration and functionality of the machine was to be tested. To measure the vertical movement, the machine was set to various speeds and would be calibrated using a handheld stopwatch to measure time at a fixed distance. Upon calibrating the speeds and establishing repeatibility, the pinch force assembly was evaluated. Here, the internal force sensor was to be calibrated and unfortunately, the machine did not come with a calibration kit or any instructions on how to calibrate the force sensor. Typically, this work could be outsourced from the manufacturer of the machine, but the product was discontinued. So, our next task was to design a calibration procedure and generate calibration equipment to confirm accuracy of the force sensor.

Pinch Clamp Force Sensor Calibration: The force clamp assembly had a relatively simple design. It consists of two Stainless Steel blocks, with movement in the horizontal direction to generate the "pinch" or "clamp" onto the sample. The blocks would simultaneously move inward together to pinch down on the sample and one of the blocks had the force sensor behind it that would measure the amount of pinch clamp force. After extensive planning and discussion on the best way to calibrate the force sensor, it was determined to design an L-bracket, that could hold calibrated weights would be sufficient. On my own time, I created a similar design as the L-Bracket used for reference of this project and perfromed an FEA to analyze how the calibrated weights would be translated into the sensor. Please see below the design on the L-Bracket, along with the FEA.

[L-Bracket Design](https://github.com/Franzvd14/Vertical-Pinch-Clamp-Force-Friction-Tester/blob/main/L%20Bracket.pdf)

It's important to understand this design was done based on my information and is not the correct design used on the actual machine.

[FEA Stress Analysis](https://github.com/Franzvd14/Vertical-Pinch-Clamp-Force-Friction-Tester/blob/main/Screenshot%202025-08-31%20171741.png)

After creating the design, FEA was performed. The applied force load was 2lbs and was a circular evenly distributed load. The fixed support was placed along the vertical bracket design, where the force sensor was located. The heat map indicates where most of the stress was located.

[FEA F_x, F_y, F_z](https://github.com/Franzvd14/Vertical-Pinch-Clamp-Force-Friction-Tester/blob/main/Screenshot%202025-08-31%20171722.png)

Here, a force analysis was done on the x,y, and z axis to understand more on how the load was distributed into the force sensor. 
