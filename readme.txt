ForceTubeVR Documentation

1 - Button

- To put on a ForceTubeVR, you only have to press the on/off button. You should see two lights from your ForceTubeVR when it is on. 

- To put it off, make sure you unplugged it and press the on/off button for 3 seconds. If a light was blinking, it should freeze when you can release the button.

2 - Battery and LED

- A little LED, always red, means the ForceTubeVR microcontroller is on.

- The other LED (the batteries level LED) is red when you have low batteries, green when it is on middle of batteries charge and white when it has more than 80% of batteries charge. 
This LED blinks (0.71 Hz) when the ForceTubeVR isn't connected (it means it is free to pair or connect) and is static when it is connected. 
It blinks very quickly (0.33 Hz) if you have a battery cell with a perilously low charge level. At this state, the ForceTubeVR should stop any connection.

- You can charge the ForceTubeVR by plugged in by USB-C. It will automatically stop the charge when the ForceTubeVR is fully charged. You can't put it off when it is plugged in.
The batteries level LED turns orange when the ForceTubeVR is plugged in and is charging. If it turns white and still plugged in, it means the batteries charge is over. 

3 - Bluetooth pairing

- To use the ForceTubeVR, you first have to put it on and to pair it by Bluetooth in your OS (Android for a Oculus Quest and Windows for other headsets).

3.1 - On Windows

- To pair it on Windows 10, plug your Bluetooth dongle in your computer, put on your ForceTubeVR and make sure it isn't connected (the batteries level LED shouldn't blink). 
Open the Windows settings, click "Devices" > "Bluetooth and other devices". Then turn on the Bluetooth if it isn't done and click "Add Bluetooth or other device" > "Bluetooth". 
When your ForceTubeVR appears in the list of available devices, click it. Wait a few seconds while your ForceTubeVR is paired to Windows.

- If your ForceTubeVR is paired on Windows but can't connect in games or Companion Application, it may be due to a pairing to the bad Bluetooth transmitter.
It is a Windows problem : Windows uses to only work with one Bluetooth transmitter, but all devices ever paired to one transmitter can't be paired to another.
This problem can occur if you have different Bluetooth transmitters installed or even if you only moved your Bluetooth dongle to a new USB port and Windows had difficulties to recognize it, asuming it is a new Bluetooth dongle even if it isn't.
So you should try to remove the ForceTubeVR to pair it again.
If you have difficulties to remove it, you should go to you Device Manager, click "View" > "Show Hidden Devices", and open the "Bluetooth" tab.
In this "Bluetooth" tab, you should uninstall all unconnected devices (they have clearer icons) by right-clicking them and selecting "Uninstall device" and restart your computer.
Once done, try to pair again your ForceTubeVR on Windows.
If you accidentally remove a device you shouldn't, try to unplug it, restart your computer and plug it again.

3.2 - On Oculus Quest

- To pair a ForceTubeVR on Oculus Quest, put the ForceTubeVR and the Oculus Quest on and, in the Oculus Quest home, click "Settings" > "See all" > "Experimental features". 
Next to "Bluetooth pairing", click "Pair". Scroll the list of devices and when you find your ForceTubeVR, click it. After some seconds, click "Pair".

4 - Play

4.1 - Native integration in games

- Some games integrated the ForceTubeVR to be natively compatible. These natively compatible games only need you have a put on paired ForceTubeVR when you launch them.
You can adjust the power and duration of ForceTubeVR feedbacks if you use the Companion Application.
For more details, go to 5.3 part.

4.2 - Backward compatibility with SteamVR

- Other games can works with ForceTubeVR if you launch them by SteamVR and you use the Companion Application.
For more details, go to 5.2 part.

5 - Companion Application for Windows

- You can download it here : https://github.com/ProTubeVR/ForceTubeVR-User-Content/raw/master/ForceTubeVR%20Companion/ForceTubeVR%20Companion%20Application.rar

- It will automatically ask you the permission to auto-update when a new version is available.

- In the Companion Application, you have 4 tabs called "Channels binding", "SteamVR Backward compatibility", "Native Game Personalization" and "Demo".
In all these tabs, you have some options, but the bottom of the window is common to all tabs.

5.1 - Channel binding

- In this tab, you can see the six channels, in six columns, used to send targeted commands to ForceTuberVR.
By default, most of games send requests to both "Rifle" channels (RifleButt and RifleBolt), but some games are designed to send requests to specifics channels. 
It enable players to apply different setups (one by channel) at the same time. It is useful if you have multiple ForceTubeVRs.

- In all these channels, you can click in "Add output" to add a ForceTubeVR. A ForceTubeVR can be placed in different channels simultaneously, it simply receive the signals from all these channels.

- You can remove a ForceTubeVR from a channel by clicking the "Remove" button below, make it rumble by clicking the "Identify" button also below, and make rumble an entire channel by clicking the channel name.

- To custom the signals received by each channel, you can click "SteamVR Compatibility" and "Natives Games" in the channel column. 
It respectively switches to the "SteamVR Backward Compatibility" and "Native Game Personalization" tabs and selects the channel to edit (you can see the selected one in the combobox "Channel" on the bottom) to match with the column where you clicked.

5.2 - SteamVR Backward Compatibility

- You can use it to spy the rumble requests sent by SteamVR to your VR controllers and transmit them to your ForceTubeVR under some conditions. It needs you keep the Companion Application open in background.
Remember when you change something here, you only do it for the selected channel. You can see it in the "Channel" comboboxe on the bottom. To edit another channel, select it in this comboboxe before.

- The "Enable backward compatibility" button let you enable or disable the SteamVR spy.

- All the following sliders are useful to properly isolate the controller rumble signals corresponding to shoots, and to traduce them into realistic ForceTubeVR feedbacks.
The "Kick power" slider let you choose the strength of the ForceTubeVR kicks generated by the backward compatibility.
The "Kick treshold" slider let you choose the minimum power required by the Companion Application to make kick the ForceTubeVR. All signals shorter will only trigger the rumble motors of the ForceTubeVR.
The "Big rumble treshold" slider let you choose the minimum power required to activate the bigger rumble motor of the ForceTubeVR. All signals weaker will only trigger the smaller rumble motor of the ForceTubeVR.
The "Minimum rumble duration" let you choose the minimum duration of a signal to transmit it. All signals shorter will be ignored.
A too high value combinated to too high shot frequencies can too much solicitate the kick motor and make you feel missfires.
It isn't the same problem with the rumble motors, that's why when they are activated by the backward compatibility, they use the same power values than in the original SteamVR controllers signals.
The "Delay betwenn shots" slider let you choose a minimum delay between two shots. After a request is transmitted, all following during the duration you choosed won't be transmitted.

- Below these sliders, there are two columns : "Left hand controller" and "Right hand controller". For each of these controllers, you have the three following options :  
The "Listen controller events" button let you choose to spy or not the events from the VR controller left or right.
The "Transmit controller to kick" button let you choose to transmit or not the events from the VR controller left or right to the kick motor (solenoid) of the ForceTubeVR.
The "Transmit controller to rumble" button let you choose to transmit or not the events from the VR controller left or right to the rumble motors of the ForceTubeVR.

5.3 - Native Game Customization

- You can use it to custom the ForceTubeVR requests sent by natively compatible games. It needs you keep the Companion Application open in background.
Remember when you change something here, you only do it for the selected channel. You can see it in the "Channel" comboboxe on the bottom. To edit another channel, select it in this comboboxe before.

- The "Enable native games customization" button let you enable or disable this function.

- The 3 next sliders values are percents, 200 means +100% (the same as x2), 100 means +0% (the same as x1) and 0 means -100% (the same as x0).
The "Native kick power multiplier" let you choose to increase or reduce the kick powers of ForceTubeVR requests from the natively compatible games.
The "Native rumble power multiplier" let you choose to increase or reduce the rumble powers of ForceTubeVR requests from the natively compatible games.
The "Native rumble duration multiplier" let you choose to increase or reduce the rumble durations of ForceTubeVR requests from the natively compatible games.

5.4 - Demo

- Here you can do all the tests you want, for example to test the behaviour of a channel or to simply show the ForceTubeVR possibilities.
Remember the requests you send from here are only sent to the selected channel. You can see it in the "Channel" comboboxe on the bottom. To target another channel, select it in this comboboxe before.

- The left and central part is like a toolkit to let you send fully custom requests to ForceTubeVR and the right column is a set of precalibrated typical requests you should often find in natively compatible games.
So the the "Custom single shot button" sends a request containing a kick if the "Enable kick" button is enabled and a rumble if the "Enable rumble" button is enabled.
The kick will have a power equal to the "Kick power" slider value. The rumble will have a power equal to the "Rumble power" slider value and a duration equal to the "Rumble duration" slider value.
If the "Cutom autoshot" button is enabled, it regularly sends a "Custom single shot" button request. The frequency (the number of shots by second) is equal to the "Autoshot frequency" slider value.

- The "Example sniper" button sends a unique powerful shot.
The "Example p90" button sends high frequency shots while enabled.
The "Example m16" button sends a burst of three little shots.
The "Example pkm" button sends powerful shots with a low frequency while enabled.
The "Example Lasergun" button triggers a increasing rumble when it is clicked the first time (simulating a power loading lasergun) and sends a powerful shot (with a rumble power relative to the loading duration) when it is clicked the second time.

5.5 - Other features

5.5.1 - ForceTubeVR Auto Research

- When the "Forcetubevr auto research" button is enabled, the Companion Application will automatically looking for all unconnected but paired ForceTubeVR in background. It is useful to quickly recover the connection after a ForceTubeVR disconnection.

- But if you have an off paired ForceTubeVR, it can cause some audio noise in Bluetooth headphone. To prevent this, unpair the off paired ForceTubeVR or disable this button.

- When you launch the Companion Application, the natively compatible games stop their ForceTubeVR researches and let the Companion Application do it for them.
So, to prevent the audio noise in Bluetooth headphones in games if you have an off paired ForceTubeVR, you have two solutions : 
Launch the Companion Application, wait for your ForceTubeVR connection and uncheck the "ForceTubeVR Auto research" button.
You can also simply unpair your off paired ForceTubeVR.

5.5.2 - Channel Comboboxe

- It shows the channel which is customized by the "SteamVR Backward Compatibility" and "Native Game Personalization" tabs and targeted by requests from the "Demo" tab.
You can change it by clicking and selecting the new one you want to edit or target. 
When you select a new channel, you should see the "SteamVR Backward Compatibility" and "Native Game Personalization" values change to the ones of the new selected channel.

5.5.3 - Display ForceTubeVR Renderer

- The "Display forcetubevr renderer" button open a tranparent window containing a ForceTubeVR picture. 
The back of the ForceTubeVR picture kicks when the Companion Application or a natively compatible game sends a kick request to your ForceTubeVR.
The picture entirely vibrates when the Companion Application or a natively compatible game sends a rumble request to your ForceTubeVR.
It is useful to easily illustrate the ForceTubeVR behavior, for example during a live streaming on Twitch.

6 - Companion Application for Oculus Quest

6.1 - Channel binding