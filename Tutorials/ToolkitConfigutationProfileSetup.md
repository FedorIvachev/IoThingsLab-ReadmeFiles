# In this tutorial you will know how to disable Diagnostics window and how to change controls for the Input Simulation Mode.
## These are the two main issues users of MRTK faced. Let's start from the first one - diagnostics window. By default, it is always in front of the user, but it can be disabled in several steps.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Oculus-2.jpg)

## 1. Select MixedRealityToolkit GameObject in the Hierarchy window and in the Inspector window clone the DefaultMixedRealityToolkitConfigurationProfile.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/ToolkitConfigurationProfileSetup-1.png)

## 2. Give a name to your new profile. Click on clone. The cloned profile will be created in Assets/MixedRealityToolkit.Generated/CustomProfiles by default.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/ToolkitConfigurationProfileSetup-2.png)

## 3. Click on the profile file and navigate to the diagnostics window. To disable the diagnostics window, uncheck the corresponding checkbox.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/ToolkitConfigurationProfileSetup-3.png)

## 4. Now there won't be any diagnostic window in front of you.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/MRTK-Oculus-1.png)

## The second problem users want to solve is Input Simulation Mode camera rotation not only by the mouse right click. Not everyone uses optical mouses, many people use touchpads instead.

## 5. Same as in step 3, navigate to the Input tab of the profile. and Clone the DefaultMixedRealityInputSystemProfile.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/ToolkitConfigurationProfileSetup-4.png)

## 6. Go to Input Data Providers->Input Simulation Service and clone the DefaultMixedRealityInputSimulationProfile. Name your profile and press the "Clone" button.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/ToolkitConfigurationProfileSetup-5.png)

## 8. Now you can change the Mouse Look Button to a specific one.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Setup-Pictures/ToolkitConfigurationProfileSetup-6.png)
