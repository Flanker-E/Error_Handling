# Error_Handling
Error handling strategy would tackles the error and the torque attribution according to the error type.<br>
The module judges the status according to the type of the four motor Errors
Re-power on and restart each motor after the whole vehicle is powered on.

Module return signals:

Error status Num: corresponding to normal, front drive, rear drive, restart, and disabled;
Restart status: indicates that the motor controller is restarting
Motor controller power supply relay RelayOut: control is closed (1 is energized and 0 is disconnected), and requires the actual state RelayIn to confirm that it has restarted.

2020/2/6 V2.0<br>
The overall view of error handling.<br>
![img](https://github.com/Flanker-E/repository_photo-gif/blob/main/Errorhandling_1.png)<br>
The ErrorMode block.<br>
![img](https://github.com/Flanker-E/repository_photo-gif/blob/main/Errorhandling_ErrorMode.png)<br>
The TX block.<br>
![img](https://github.com/Flanker-E/repository_photo-gif/blob/main/Errorhandling_TX.png)<br>
The ErrorType block.<br>
![img](https://github.com/Flanker-E/repository_photo-gif/blob/main/Errorhandling_ErrorType.png)<br>
