**Introduction :**

  The development of the MARS vehicle has been achieved through the integration of a dual microcontroller system, 
featuring both a Raspberry Pi and an Arduino. This innovative setup has enabled the MARS vehicle to harness the strengths of both platforms,
thereby enhancing its overall functionality and control capabilities.
  
  The Raspberry Pi serves as the primary controller, running on a Linux environment that provides a robust foundation for executing high-level tasks and intricate algorithms.
On the other hand, the Arduino, operating under the Arduino IDE ARM version, specializes in low-level hardware control and real-time operations.
  
  A pivotal component of this dual microcontroller setup is the establishment of seamless communication between the Raspberry Pi and the Arduino.
This connectivity is achieved through a reliable serial connection, allowing for the exchange of critical data and instructions between the two controllers.

  This collaborative synergy between the Raspberry Pi and Arduino empowers the MARS vehicle with a versatile and powerful computing platform,
capable of executing complex maneuvers, processing sensor data, and responding to dynamic environmental conditions with precision and efficiency.

**C Coding :**

  The code is structured into distinct sections, each serving a specific purpose within the control system of the servo motor and gyro sensor.

**Section 1: Library Imports**
  The first segment encompasses the inclusion of libraries essential for regulating servo motor movement and processing gyro sensor data.

**Section 2: Global Variables**
  In the subsequent portion, we define global variables that bear programmatically significant names. For example, variables like "forward" dictate the vehicle's forward speed,
while others such as "backward" serve analogous roles.

**Section 3: Function Definitions**
  The third section is dedicated to function definitions, with particular emphasis on pivotal functions. Notably, the "Left()" and "Right()" functions
ascertain the vehicle's directional adjustments by analyzing input from Ultrasonic Sensors. These functions operate on the principle that a counterclockwise turn is indicated 
by a substantial reading from the left Ultrasonic sensor, whereas a clockwise turn relies on a similar reading from the right sensor.

  The "readul()" function is designed to read data from all Ultrasonic sensors. In certain scenarios, specialized "readdistance()" functions are employed to individually read specific
Ultrasonic sensors, denoted by directions such as 'F' for front, 'R' for right, 'L' for left, 'N' for back-left, and 'M' for back-right.

  The "setup()" function is responsible for configuring necessary parameters, while the primary code logic resides within the "loop()" function.
Notably, the gyroscope sensor plays a crucial role in controlling the vehicle's orientation to achieve the desired angle.
Additionally, a path-tuning function is integrated to center the vehicle on the designated path.

  Furthermore, the code incorporates a function for serial communication, receiving instructions from a Raspberry Pi controller. It also includes conditional statements to guide 
the vehicle's actions upon detecting green and red obstacles in accordance with game requirements. Furthermore, auxiliary functions are integrated to facilitate precise
vehicle rotation at arbitrary angles and to manage steering angles effectively.

  In summary, the code architecture is well-organized into clear sections, with each function serving a specific and well-defined role in ensuring the precise control and maneuvering
of the vehicle.

**Python Coding:**

  The Raspberry Pi's native Python environment was leveraged to orchestrate camera operations and image processing. This robust pipeline enabled the extraction of essential information from captured images.

Color Space Transformation:
  Initially, we conducted a critical transformation of the image color scheme from RGB to the HSV (Hue, Saturation, Value) space.
This alteration set the stage for precise color-based analysis.

Color Mask Creation:
  Subsequently, we meticulously crafted color masks within the HSV system. These masks served to define the specific color ranges corresponding to green and red hues.
The masks were instrumental in pinpointing relevant regions in the images.

Region Extraction with OpenCV:
  Harnessing the capabilities of the OpenCV library, we embarked on the process of extracting regions that aligned with the predetermined color masks.
This step enabled us to isolate areas of interest within the images.

Area Extraction with Mask Consideration:
  Further refining our analysis, we employed specialized functions to isolate and quantify regions that adhered to the specified masks.
Careful attention was paid to these regions' rectangular shapes, ensuring accurate data extraction.

Serial Communication:
  Establishing seamless communication between the Raspberry Pi and the Arduino was of paramount importance. To achieve this,
we employed the serial library to connect the Raspberry Pi controller to the Arduino through the serial port.

Command Dispatch:
  In the final stage, we transmitted meticulously crafted commands through the Arduino's serial port. These commands served as directives, 
prompting the Arduino to execute precise actions in response to the information extracted from the images.

  This comprehensive image processing pipeline, seamlessly integrated with serial communication and precise command execution,
underscores our commitment to achieving robust and efficient control within the system. It is a testament to our dedication to leveraging 
cutting-edge technology and methodologies to accomplish our project's objectives.

  In summary, the MARS vehicle's success lies in its teamwork between a Raspberry Pi and an Arduino, supported by smart C and Python coding.
This combination enables the vehicle to do impressive things like navigating, sensing obstacles, and following paths with precision.
It's all about using the latest tech and clever code to make our project work really well.




