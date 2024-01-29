# gesture-vocalizer

Objective: Develop a Gesture Vocalizer that translates various hand gestures into sounds, serving as a medium for disabled individuals to convey messages effectively.  

LIST OF HARDWARE COMPONENTS
1. Arduino UNO Microcontroller
3. Flex Sensor
4. 16*2 LCD Display
5. Jumper Wires
6. Li-ion battery or cable for providing power
7. Glove
8. HC-05 Bluetooth Module
9. MPU6050 Accelerometer

working:
The flex sensor measures the bending of fingers according to gesture and outputs change in resistances corresponding to the amount of bending. Accelerometer sensor measures the linear movements of hand in X-axis and outputs different values of X corresponding to the movement in X-axis. All the data from sensors are then processed on Arduino UNO involves combination of all the sensor outputs in order to match the resultant output with pre-stored values of different signs regarding the alphabets. For this, appropriate ranges are set for each alphabet and the words that can be recognized with single hand based on the measured data obtained from repeated measurements. A Bluetooth module is connected to Arduino UNO. The Processed data are then transferred to the Bluetooth module (transmitter) obtained in string format. The
Android mobile also have an inbuilt Bluetooth capability. These two Bluetooth devices are then paired, and string is transmitted to Android mobile. Android mobile receives data via Bluetooth in bytes format, convert them into string. Finally, the string is converted into voice using the text to speech application of Android mobile.This overall system is mounted over a normal glove for easy handling and recognizes
the hand gestures accurately.
