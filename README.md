This app serves as a receiver of navigation commands from external sources via the internet (initially, a software on a server will have the drone's navigation intelligence), and translates the commands to send to the remote control of the DRONE using the DJI SDK, so that the control communicates with the DRONE by sending the appropriate movement command. However, so far the SDK has not been imported into the project. The app only pulls the commands that were sent from the RabbitMQ server and simulates the translation of the command by animating a set of arrows displayed on the device screen.

The implementation of the communication with the RabbitMQ server (which can be used for other purposes) is all in the MensageriaThread.java class.

INSTALLATION:

(Option 1) Copy the APK located in /app/build/outputs/apk/debug/app-debug.apk to your Android mobile device and install it. Note: it is necessary to enable the installation of external sources in the Android configuration. It will give a warning if it is not.

(Option 2) Use Android Studio on a PC with the Android phone connected via USB, and run Run / Run APP. Note: it is necessary to enable debugging mode in the Android settings. It will give a warning if it is not.