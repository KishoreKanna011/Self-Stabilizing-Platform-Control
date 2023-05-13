# Self-Stabilizing-Platform-Control

In this code, the MPU6050 library is used to interface with the MPU6050 sensor. The sensor readings are used to calculate the pitch and roll angles. The current angle is calculated by averaging the pitch and roll angles. The motor pin is defined as pin 9, and the target angle is set to 0 degrees (the original position).

In the loop() function, the current angle is read and compared to the target angle. If the current angle is greater than the target angle, indicating a clockwise tilt, the motor pin is set to HIGH to rotate the motor anticlockwise. Similarly, if the current angle is less than the target angle, indicating an anticlockwise tilt, the motor pin is set to LOW to rotate the motor clockwise.

Please note that you may need to calibrate the MPU6050 sensor and adjust the delays according to your specific setup.

Please make sure you have the updated MPU6050 library installed in your Arduino IDE. You may need to download the latest version from the library manager or from the library's official repository.
