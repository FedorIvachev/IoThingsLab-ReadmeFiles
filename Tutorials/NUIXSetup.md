# Unity + Oculus + Mixed Reality Toolkit + NUIX-Studio Setup

## Table of contents
* [General info](#general-info)
* [Required software and hardware](#required-software-and-hardware)
* [Unity Setup](#unity-setup)
* [Mixed Reality Toolkit Setup](#mixed-reality-toolkit-setup)
* [NUIX-Studio Setup](#nuix-studio-setup)


## General info
In this tutorial you will learn how to setup Unity to work with Oculus Quest Virtual Reality Headsets.\
Firstly,
* [Unity](https://unity.com) is a game engine, it has plenty of tutorials and is often used by VR researchers;
* [Oculus Quest / Quest 2](https://www.oculus.com) are the latest generation Virtual Reality Headsets made by Facebook. Oculus SDK provides rich functionality for hands and controllers recognition and VR tools;
* [Mixed Reality Toolkit](https://github.com/microsoft/MixedRealityToolkit-Unity) provides components and features to be used by the researchers such as buttons, sliders and other UI elements;
* [NUIX-Studio](https://github.com/VRSimulator/NUIX-Studio-APP) is a platform which can be used to integrate the IoT software inside Virtual Reality. It helps testing AIoT scenarios inside XR (Virtual, Augmented, Mixed Realities).

## Required software and hardware
| [![Unity](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK170802_Short_18.png)](https://unity3d.com/get-unity/download/archive) [Unity 2020 LTS](https://unity3d.com/get-unity/download/archive)| [![Visual Studio 2019](https://camo.githubusercontent.com/e5e43f29fcf61f4180ee4b52b1451bf35c0765e135b5bef1578c4abe320e62d3/68747470733a2f2f646f63732e6d6963726f736f66742e636f6d2f77696e646f77732f6d697865642d7265616c6974792f6d72746b2d756e6974792f66656174757265732f696d616765732f4d52544b3137303830325f53686f72745f31392e706e67)](http://dev.windows.com/downloads) [Visual Studio 2019 (install with Unity)](http://dev.windows.com/downloads)| [![Oculus Quest 1/2](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK170802_Short_20.png)](https://www.oculus.com/quest-2/) [Oculus Quest 1/2](https://www.oculus.com/quest-2/)|
| :--- | :--- | :--- |

## Unity Setup

### 1. Download and Install [Unity HUB](https://store.unity.com/download?ref=personal).
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/UNITY-Setup-2.png)

### 2.1 Register a personal account at [Unity](https://unity.com).
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/License-1.png)

### 2.2 Log in to your account in Unity Hub.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/License-2.png)

### 2.3 Select *Activate a new license*.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/License-3.png)

### 2.4 Confirm the user agreement.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/License-4.png)

### 2.5 The license is added to Unity Hub.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/License-5.png)

### 3. Proceed to the Installs tab.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/UNITY-Setup-4.png)

### 4. Add Unity version 2020, click Next.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/UNITY-Setup-5.png)

### 5. Select Visual Studio, Android Build Support and Documentation. Click Next and wait for the Unity version to be installed.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/UNITY-Setup-6.png)
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/UNITY-Setup-1.png)

### 6. Go to the Projects tab and create a new project with a 3D template.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/UNITY-Setup-7.png)
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/UNITY-Setup-7-1.png)

### 7. Press Play button to check if there are no errors.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/UNITY-Setup-8.png)

### 8. Press the play button again to finish the project running in the Play mode. You can exit this project and safely delete it.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/UNITY-Setup-9.png)

## Mixed Reality Toolkit Setup

### To save your time, Mixed Reality Toolkit with already configured Oculus Integration package can be [downloaded as a project from Github](https://github.com/FedorIvachev/OculusMRTKUnityProject/archive/refs/heads/master.zip). If you want to add MRTK and Oculus integrations into an existing project, you can follow the full setup procedure, which can be found at [MRTK-Setup page](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/MRTKSetup.md).

### 1. Unpack the downloaded archive and then open the downloaded project using Unity HUB. 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-1-1.png)

### 1.1 If you are using macOS, you will receive the following warning. You can either press "Move to bin" or "Cancel". For Windows there may be no such issue.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-1-2.png)

### 1.2 If you press cancel, then select "Allow Anyway" in your security settings. 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-1-3.png)

### 1.3 Then select "Open". 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-1-4.png)

### 2. After the project has been imported, navigate to Assets/MRTK/Examples/Demos/HandTracking/Scenes and Double click on the HandInteractionExamples.unity scene file.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-11.png)

### 2.1. Press the play button. 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-12.png)

### 3. You have entered the input simulation mode. You can move around the scene by pressing WASD, QE keys, Shift and Space buttons can be used for simulating hands in VR, and use left-click to simulate the pinch gesture. Press the Play button again to exit the Play mode.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-13.png)

### 4. Navigate to File->Build Settings.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-14.png)

### 5. Switch platform to Android. This action may take several minutes.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-15.png)

### 6. Next, click on Add Open Scenes and Select the Oculus Quest inside the Devices List. If Oculus Quest is not recognized in the list, it is either not turned on or the [Development mode](https://developer.oculus.com/documentation/native/android/mobile-device-setup/) is not enabled on it.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-16.png)

### 7. Click on the Build and Run button, give your build a name and then wait for several minutes. The first build takes more time than later builds. 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-17.png)

### 8. After the build is completed, check in the Console tab (in Unity) if there are errors. Put on your Oculus Quest 2 and test the scene.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-18.png)

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Oculus-1.png)



## NUIX-Studio setup

### 1. [NUIX-Studio](https://github.com/VRSimulator/NUIX-Studio-APP) will soon be distributed as a Unity Package. The installation procedure and tutorial can be found [here](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIXTutorial.md).


