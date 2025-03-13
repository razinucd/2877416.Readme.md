**Introduction**
This project is a motion detection security camera system meant to give realt time surveillance using a Raspberry Pi and a webcam. It continuously monitors an area for any movement showing that the surrounding areas stay under watch at all times. As soon as motion is detected, the system plays a warning beep, records a short video, and sends an email alert with the footage attached. The system is automatic and begins functioning as as when the Raspberry Pi is powered on stopping the need for turning it on manually . This makes it highly reliable for  security monitoring without user intervention.

The system works by examining individual frames from the camera using OpenCV. When differences between frames indicate movement, the program sees the motion and triggers the  actions. A beep sound is played to alert anyone nearby and scare away intruders, and a short video of the detected movement is recorded and stored. also, an email alert is sent to a set address based off the user, showing that the user is notified even if they are not physically there. This improves alerts and video evidence improves security and gives an good way to monitor spaces without being home.

**Purpose and Usage**
The main point of this project is to be  a security camera system that can be used in homes offices or anywhere that needs  monitoring at all times. It is designed to see  movement, alert the intruder through an obnoxious beep signal, and give visual proof of any unwanted activity. By automatically recording a video and sending alerts, it ensures that no motion goes unnoticed. This makes it useful for protecting property, monitoring sensitive areas, and keeping track of movements in places where security is a concern.

This system is good for home security, allowing homeowners to monitor entrances, garages, and driveways. It can also be used in workplaces to keep see office spaces after hours. For businesses, it adds an more  surveillance by recording any unusual activity in storage rooms or areas of no entry.

**How It Works**
The system continuously captures video frames from the connected camera and processes using OpenCV. it compares the difference between frames and determines whether any movement has occurred. If  movement is detected, the system starts the alert sequence. A beep sound is played through the Raspberry Pi speaker or  audio output to give a immediate warning. The program then records a short video clip of the detected motion and saves it in a  folder. Once the video is saved  the system automatically sends an email notification with the recorded footage attached, that provides the date and time of said motion

The email alert function makes sure that the user knows whats going even when they are away. The  system is programmed to start functioning as soon as the Raspberry Pi is powered on, making it a useful security solution. There is no need to manually activate or configure the program each time, as it runs automatically in the background. This guarantees uninterrupted surveillance and enhances the reliability of the system.

**The code**
The motion detection system consists of three main scripts ( motionDetect.py, mailSend.py, and soundModule.py). The motionDetect.py script uses OpenCV to detect video frames and  motion by comparing  frames. If motion is found, the system records a short video, saves it and triggers both an  beep and an email alert. The dimensions for motion detection were adapted from a guide found on Instructables, which helped optimize accuracy. The mailSend.py script is for the email notifications The code for sending emails was sourced from the same Instructables guide, which gives a fast way to add SMTP for alerts. This script attaches the recorded video and sends it to a recipient, making sure that users are informed of detected motion in real time. The soundModule.py script generates a beep sound when motion is seen using a speaker to give a warning. This alerts anyone nearby while the system  records and sends footage .




**Conclusion**
This project is an automated motion security system using a Raspberry Pi. It detects movement, records video, plays an alert sound, and sends email notifications. The system runs continuously making it a good surveillance solution for many security purposes.

**Referance list**
Instructables, 2018. Raspberry Pi Motion Detection Security Camera. Available at: https://www.instructables.com/Raspberry-Pi-Motion-Detection-Security-Camera/ [Accessed 12 March 2025].

YouTube, 2021. Raspberry Pi Motion Detection Security Camera [video online]. Available at: https://www.youtube.com/watch?v=QzVYnG-WaM4 [Accessed 12 March 2025].
