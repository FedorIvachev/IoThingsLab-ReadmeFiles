# Unity + Oculus + Mixed Reality Toolkit + NUIX-Studio Setup

## Table of contents
* [General info](#general-info)
* [Required software and hardware](#required-software-and-hardware)
* [Unity Setup](#unity-setup)
* [Mixed Reality Toolkit Setup](#mrtk-setup)
* [NUIX-Studio Setup](#nuix-setup)
* [Oculus Integration Setup](#oculus-setup)


## General info
In this tutorial you will learn how to setup Unity to work with Oculus Quest Virtual Reality Headsets.\
Firstly,
* [Unity](https://unity.com) is a game engine, it has plenty of tutorials and is often used by VR researchers;
* [Oculus Quest / Quest 2](https://www.oculus.com) are the latest generation Virtual Reality Headsets made by Facebook. Oculus SDK provides rich functionality for hands and controllers recognition and VR tools;
* [Mixed Reality Toolkit](https://github.com/microsoft/MixedRealityToolkit-Unity) provides components and features to be used by the researchers such as buttons, sliders and other UI elements;
* [NUIX-Studio](https://github.com/VRSimulator/NUIX-Studio-APP) is a platform which can be used to integrate the IoT software inside Virtual Reality. It helps testing AIoT scenarios inside XR (Virtual, Augmented, Mixed Realities).

## Required software and hardware
| [![Unity](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK170802_Short_18.png)](https://unity3d.com/get-unity/download/archive) [Unity 2020 LTS](https://unity3d.com/get-unity/download/archive)| [![Visual Studio 2019](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK170802_Short_19.png)](http://dev.windows.com/downloads) [Visual Studio 2019 (install with Unity)](http://dev.windows.com/downloads)| [![Oculus Quest 1/2](https://docs.microsoft.com/windows/mixed-reality/mrtk-unity/features/images/MRTK170802_Short_20.png)](https://www.oculus.com/quest-2/) [Oculus Quest 1/2](https://www.oculus.com/quest-2/)|
| :--- | :--- | :--- |

## Unity Setup

### 1. Download and Install [Unity HUB](https://store.unity.com/download?ref=personal).
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/UNITY-Setup-2.png)

### 2. Inside Unity HUB preferences, activate a new License (you can register a personal account at [Unity](https://unity.com)).
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/UNITY-Setup-3.png)

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

### 8. Press the play button again to finish the project running in the Play mode.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/UNITY-Setup-9.png)

## Mixed Reality Toolkit install

### 1. Mixed Reality Toolkit can be downloaded from the [Github repository releases](https://github.com/microsoft/MixedRealityToolkit-Unity/releases). Follow the steps in the tutorial for the latest version of MRTK(Mixed Reality Toolkit). Mixed Reality Feature Tool can be used only in Windows, so if you are using macOS, download the attached .unitypackage files. However, you can follow the same steps below on Windows as well.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-1.png)

### 2. If you are using macOS, import the Foundation, Extensions and Examples unitypackages one by one into your created projected.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-2.png)

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-3.png)

### 3. After the import of the Foundation Package (which you imported first) MRTK Project configurator window will pop-up. Select the non-OpenXR option.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-4.png)

### 4. Press Show Settings.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-5.png)

### 5. Inside Android Build target tab select the Oculus Plug-In provider.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-6.png)

### 6. Close the project settings and select Oculus Audio Spatializer and click on Apply button.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-7.png)

### 7. Then click Next.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-8.png)

### 8. Import TMP Essentials.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-9.png)

### 9. Click on Done. After you import Extensions and Examples packages this window will pop-up again, but you can just select "Always skip the Setup".
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-10.png)

### 10. After the Mixed Reality Toolkit packages have been imported, navigate to Assets/MRTK/Examples/Demos/HandTracking/Scenes and Double click on the HandInteractionExamples.unity scene file.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-11.png)

### 11. Press the play button. 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-12.png)

### 12. You have entered the input simulation mode. You can move around the scene by pressing WASD, QE keys, Shift and Space buttons can be used for simulating hands in VR, and use left-click to simulate the pinch gesture. Press the Play button again to exit the Play mode.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-13.png)

### 13. Next, Click on the MixedRealityToolkit GameObject in the Hierarchy tab, and then change the Configuration Profile to DefaultMixedRealityToolkitConfigurationProfile. Press Ctrl-S to save the changes.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-13-1.png)

### 14. Navigate to File->Build Settings.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-14.png)

### 15. Switch platform to Android. This action may take several minutes.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-15.png)

### 16. Next, click on Add Open Scenes and Select the Oculus Quest inside the Devices List. If Oculus Quest is not recognized in the list, it is either it is not turned on or the Development mode is not enabled on it.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-16.png)

### 17. Click on Build and Run button, give your build a name and then wait for several minutes. The first build takes more time than later builds. 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-17.png)

### 18. After the build is completed, check in the Console tab (in Unity) if there are no errors. Put on your Oculus Quest 2 and test the scene.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-18.png)


### Now you can test your project inside Virtual Reality.





