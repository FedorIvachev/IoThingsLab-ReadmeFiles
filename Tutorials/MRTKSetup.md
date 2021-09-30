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

### 17. In your blrowser, go to the [Oculus integration page](https://assetstore.unity.com/packages/tools/integration/oculus-integration-82022) and add it to your assets.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-16-1.png)

### 18. In Unity, go to the Window->Package Manager and import the Oculus Integration package. To see it on the list, you need to select "Packages: My Assets".
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-16-2.png)

### 19. Next, navigate to Mixed Reality->Toolkit->Utilities->Oculus and click on "Integrate Oculus Integration Unity Modules".
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-16-3.png)

### 20. Click on the Assets->Oculus->OculusProjectConfig.asset and set Hand Tracking support to Controllers and Hands.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-16-4.png)

### 17. Navigate to File->Build Settings and click on Build and Run button, give your build a name and then wait for several minutes. The first build takes more time than later builds. 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-17.png)

### 18. After the build is completed, check in the Console tab (in Unity) if there are no errors.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Setup-18.png)

### 19. Put on your Oculus Quest 2 and test the scene. You must be able to move in 6DOF and register your hands movements.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Oculus-1.png)

See how to disable diagnostics Window and how to change the mouse look button in Input Simulation mode in the [next tutorial](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/ToolkitConfigutationProfileSetup.md).
