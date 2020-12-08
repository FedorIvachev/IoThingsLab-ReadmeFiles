Check if SteamVR is installed

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/1.png)

And Oculus is installed (only required for Oculus Quest support, not needed for HTC Vive and other headsets)

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/2.png)

Check if you SteamVR environment works

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/7.png)

Download Unity Hub

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/3.png)

Add a Unity Version (2019.4)

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/4.png)

Checkbox the  Windows Build Support
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/5.png)

Add a new project

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/8.png)

Select 3D template
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/9.png)

Go to [Mixed Reality Toolkit installation](https://microsoft.github.io/MixedRealityToolkit-Unity/Documentation/Installation.html). 
Download the .unitypackage files from MRTK release page.

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/6.png)

Import them into your project (Foundation, then Extensions, then Examples)

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/10.png)

Click Apply (and every time you see this message, click apply)

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/11.png)

Open any scene inside MRTK examples (for example, the one from screenshot)

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/12.png)

Click import TMP essentials

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/13.png)

Next go to the asset store inside Unity, search for SteamVR Plugin, click download
 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/15.png)

And then import

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/16.png)

Click Accept all - OK

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/17.png)

Go into build settings, click add open scenes, check if PC, Mac & Linux Standalone platform is selected. Click Build and Run

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/18.png)

Put On your Headset. SteamVR should be running and you should be able to press some buttons in VR using this demo

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/19.png)

Congratulations, you have MRTK running on SteamVR

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/20.png)

Now importing IoThingsLab. Go to [releases](https://github.com/VRSimulator/IoThingsLab/releases/) and download the latest IoThingsLab-Together.unitypackage

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/21.png)

Import it

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/22.png)

Accept all

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/23.png)

Open the Client Scene (Assets/com.tsinghua.iotvrp/Scenes)

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/24.png)

This material is missing (because it was using Oculus plugin). Let's try to fix it ourselves for now. Select the FloorPlane

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/25.png)

And change the material to default

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/26.png)

Go to MixedRealityToolkit.

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/27.png)

Select DefaultMixedRealityToolkitConfigurationProfile as the Active profile

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/28.png)

Go to build settings again.

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/29.png)

Select Add open scenes, remove the previous scene. Click Build and Run

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/30.png)

Congrats on running IoThingsLab on SteamVR
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Readme/Files/SteamVRSetupTutorial/Inked31_LI.jpg)
