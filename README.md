MARS.

Overview:

The main objective of our self-driving vehicle is to participate in the World Robot Olympiad and prepare it to overcome all obstacles inside the racetrack using specific techniques and taking advantage of the strengths of each team member.

Our project description:

Our self-driving vehicle has four wheels and we controlled, these four wheels with a steering that we connected to a single motor and used four-wheel system to drive the wheels, as well as the rear differential and front differential gears to distribute the engine power to the four wheels and other luxuries such as the transmission and a rear drive shaft all to build a strong base for our vehicle.

To control our vehicle, we used an Arduino controller which connected to a Raspberry Pi 4 computer, and we added the Arduino to the Raspberry Pi4 in order to our neediness to a controller with a mini-computer because we cannot implement our plan without the presence of both Raspberry Pi 4 and Arduino.

The method of work that we worked to implement between the Arduino and the Raspberry Pi 4 is to make the vehicle successful was through the Arduino controlling the movement of the car’s wheels and the sensors that we added and everything that is in the chassis of the vehicle, and the function of the Raspberry Pi 4 is to take the data from the camera ( obstacles locations ) and send it to the Arduino ,that means that the Raspberry Pi 4 sends the signals which were received from the camera to the Arduino , so the Arduino analyzes it and sends it to the system and we preferred to use the Raspberry Pi 4 camera instead of connecting an external camera to get the fastest response, as the Raspberry camera's response is faster than connecting an external camera via the ‘USB port’, But we couldn't do that and we used a camera with a USB port because the Raspberry Pi 4 camera malfunctioned and we didn't have much time left to get another one, so we replaced it with another USB camera.

The programming languages that we used were Python and C, where we used Python in Raspberry Pi 4 on the Linux software using the Thonny IDE “programming environment “ to determine the locations and colors of obstacles in front of it through the use of the OpenCV library In order to overcome the problem of different color’s limits from one place to another, As we have entered all the shades of red and green colors and we have done many experiments on the camera reading colors in all different lighting conditions and in many other circumstances in order to avoid any defect that may face us during racing, in addition to using the camera to determine the distance between the vehicle and the obstacle in front of it "any measurement of the dimensions of the objects that have been read", and when the car sees the obstacle in front of it, the Raspberry Pi 4 outputs a print command that tells us to go left or right (Depending on whether the color in front of it is green or red), then send this command to Arduino and we used C on Arduino to receive data from the Raspberry Pi 4 and give commands to move the bodywork.

The Arduino will receive the data from the Raspberry Pi 4 and will receive the data from the sensors we have added to ensure that the car is running correctly. Since we used two colour sensors to determine the direction of the vehicle , if it is clockwise or not by reading the orange line and the blue line on the race ground , The second sensor we added was the ultrasonic distance sensor to measure the distance between the vehicle with the outer wall and the distance between the vehicle with the inner wall and In order to avoid collision of the vehicle with the inner wall or the outer wall we have added three of this sensor where we put one on the right side, one on the left side and one on the front of the vehicle to support our vehicle and to avoid any unexpected mistakes and to confirm that, we have put a gyroscope to confirm the needed goal .

We have also used a drive motor to give high power to the motor by using the control system (the Arduino) and servo motor for two main reasons. The first one is to stick with the rules because it’s the best available choice to use, the second reason is to rotate the vehicle and push the front part of it when turning at an appropriate angle.

The power sources that we used were a twelve-volt power bank and five-volt rechargeable batteries. We connected each power source with the appropriate part. We connected the power bank with Arduino and the rechargeable batteries with Raspberry Pi 4. We used two types of power sources so that all parts of the vehicle will be in the highest quality possible.

We put all these electronic parts on a plastic base and connected them with thermal silicone, we tried to make external chassis out of plastic but the weight limit of the World Robot Olympiad rules stopped us from doing it , so we decided to use a three-dimensional printer to print the top of the car to save space and to facilitate the process of maintaining the wiring later , And because it saves a lot of weight for the car.

And to start running our vehicle we have put push button to start the vehicle journey and it’s supposed to stop atomically after finishing the three full rounds.

The measurements of our vehicle:

Our vehicle is only 14 centimeters high, about 19 centimeters wide, about 26 centimeters long, and the weight of the car does not exceed 1400 grams, which follows the World Robot Olympiad Rules.
