# NUIX-Studio Tutorial - Create IoT device

## Lets create an IoT device. This tutorial is the second part of the NUIX-Studio tutorial series. The first part can be found [here](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIXTutorial.md).

### 1. Firstly, create a new scene.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-1.png)

### 2. An empty scene should be created.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-2.png)

### 3. Add floor to the scene.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-3.png)

### 4. Let's drag the PC prefab to this scene.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-4.png)

### 5. After dragging the prefab, it is better to unpack it completely.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-5.png)

### 6. Adjust the PC position to be on a comfortable height. Select Mixed Reality -> Toolkit->Add to scene and Configure, same as in previous tutorials. Se the configuration Profile in the MixedRealityToolkit Gameobject.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-6.png)

### 7. I deciced to take a table prefab from Unity Asset store. You can add assets to your projects through [Unity website](assetstore.unity.com).
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-7.png)

### 8. Imported this asset.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-8.png)

### 9. Adjusted the table and PC positions.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-9.png)

### 10. And deleted the directional light since later I will use Point Light in a lamp.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-10.png)

### 11. The lamp is taken from the provided prefabs. It has already a light component attached. However, the lamp can not be rotated. Let's fix it.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-11.png)

### 12. Firstly, select the upper part of the lamp with a selection tool. Right click on the selected gameobject inside the hierarchy - Create empty parent gameobject. I named it "UpperPart". For the rest of the gameobjects, I put them inside another parent gameobjects and named it "LowerPart".
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-12.png)

### 13. Drag and drop the Button prefab. Buttons are located at Assets/MRTK/Features/UX/Interactable/Prefabs. Each Interactable (such as buttons, switches) has an OnClick component. You can edit it to call a specific method. Here I call LampRotator script, which performs a smooth rotation of the lamp. After pressing the play button or testing the APP on Oculus, user just needs to press a button to rotate the lamp.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-13.png)

### 14. Next, lets add speech control to the lamp. Firstly, drag a SpeechRecognition gameobject to the scene.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-15.png)

### 15. One of the children of this GameObject is NUIX Speech recognition. I decided to not make it complex, so you have more freedom in developing your own specific speech recognition logic. However, if you just want to perform actions by special keywords, this recognizer should be enough. For each type of action, create a GameObject with a wordAction component attached to it. Drag each of the wordAction gameobjects to the trigger words elements.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-16.png)

### 16. Inside the wordAction components, register the trigger words and select the actions to be performed. Here I change the light range to 0 when user says "Off", and back to normal when user says "ON". Press Build and run to test the speech recognition. The speech recognition is continious, so you don't need to press button to run the speech recognition every time. 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-17.png)

### 17. Let's make the lamp movable. Firstly, we need to add a Box collider component to it.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-18.png)

### 18. After adding the box collider component add object manipulator component.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-19.png)

### 19. The standart unity Light class does not provide methods to change the light's color. So let's do it ourselves by creating this script.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-20.png)

### 20. Attach the light changer script to the Light inside our Lamp. The Light field either can be left empty or you can drag the light from the hierarchy window inside it.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-21.png)

### 21. Attach a contact widget script onto the Lamp. Let's say we want the lamp to change color to red automatically when the keyboard is close enough to it. We just drag the keyboard gameobject from hierarchy into the Connected Item Translate field and set the available distance. Same as before, actions are assigned when the sensor is triggered (here when the keyboard is far enough from the lamp). We move the lamp closer to the table and can see that the lamp changed its light color to red.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-22.png)

### 22. We have created a smart device. Firstly, the lamp can be rotated by pressing a button. Secondly, It can be turned On and Off by Voice commands. Thirdly, It changes its color when is close enough to the keyboard. Next we want to share this IoT device to another student, so he adds more voice commands and more possible interactions. For example, the lamp can become controlled by keyboard shortcus when it is close to keyboard, or when it is activated for it by a voice command. To share the created IoT device, create a folder, and drag the gameobjects from the scene One by One inside this folder.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-23.png)

### 23. Next, select Export Package.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-24.png)

### 24. Checkbox only the scripts and prefabs you have created. 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-25.png)

### 25. Click export, give your IoT device a name.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-26.png)

### 26. Import other IoT devices same as any .unitypackage file by Import package->Custom Package.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-2-Pictures/NUIX-Tutorial-2-27.png)


## In the next tutorial you will know about each of the items for creating IoT devices NUIX studio provides.
