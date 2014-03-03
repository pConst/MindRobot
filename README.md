#lego_mindstorms_robot
###Lego Mindstorms NXT robot with Bluetooth, IR control and Autonomous mode


* Robot acts in three modes:
    * IR remote conrol
	* Bluetooth remote control
	* Autonomous mode
* Mode is selected by pressing left (most likely???) button on a brick  

* **IR remote mode** uses standart transmitter and receiver - nothing special here. To get forvard move press LeftUp + RightUp buttons
* **Bluetooth remote mode** expects you to use [Bluetooth Serial Controller](https://play.google.com/store/apps/details?id=mBluetoothSerialController.nomal&hl=en) application for Android. Complete configuration file for the app is in **Controller Backup** directory of the project. To get forvard move press LeftUp + RightUp buttons. Don`t forget to connect first!
* **Autonomous mode** - not ready

####Mindstorms NXT Bluetooth interface:
Every button press in Bluetooth Serial Controller app initiates sending one of folowing HEX sequences. Protocol is not hard to reverse - it`s obvious!

	0C000100819E0261000300313000
	0C000100819E0261000300323000
	0C000100819E0261000300333000
	0C000100819E0261000300343000

In Minstorms studio this sequences get processed by standard text messaging receive block. See ~~code~~ graphical diagram for details.

####TODO:
* Autonomous mode. Robot should explore environs and "map" plases into his memory, then return back to the base and show collected data )))
* Robot photos and videos
* Take over the world
