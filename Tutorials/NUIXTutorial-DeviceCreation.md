# NUIX-Studio Tutorial - Create IoT device

## Lets create an IoT device. This tutorial is the second part of the NUIX-Studio tutorial series. The first part can be found [here](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIXTutorial.md). You need to git clone the NUIX-Studio [repository](https://github.com/VRSimulator/NUIX-Studio-APP) inside the Assets folder of your project.

### 1. Firstly, select a scene.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-1.png)

### 2. Drag a device prefab into the scene.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-2.png)

### 3. You need to unpack it completely because we need only one GameObject.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-3.png)

### 4. Drag the Camera Gameobject outside of the parent GameObject.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-4.png)

### 5. Delete the "PC" GameObject.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-5.png)

### 6. Adjust the camera position.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-6.png)

### 7. Drag the virtual camera tool from the NUIX-interactable prefabs folder. This camera records an image into a Texture, which you can use for later analyzing.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-7.png)

### 8. For default, the camera image texture is used by a video tool. Drag the prefab into the scene and adjust its position. Unpack both of the prefabs completely.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-8.png)

### 9. Next, locate the Contact sensor GameObject under your desk. The contact sensor will be used to turn the display on the desk On and Off.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-9.png)

### 10. Click on the desk GameObject. It will become highlighted in the hierarchy window. Drag it to the top of the list and Unpack completely. 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-10.png)

### 11. Do the same with the chair and set the sensors as the children of the selected chair and desk. When you move the chair and desk, the sensors will move together with them.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-11.png)

### 12. Next, set the static component of the chair and desk to false (and select Yes for their children). To move the chair, you need to add two components to it (on the right side): the first one is Mesh Collider, and the second one is Object Manipulator.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-12.png)

![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-12-1.png)

### 13. In the Contact Sensor component, you need to set the available distance to trigger the sensor. Once the two sensors are far enough, a Unity Action is performed.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-13.png)

### 14. Press on the plus button and drag the Display GameObject from the hierarchy window into the selection field. In this example, we set the meshrenderer component to false, so the screen dissapears once the chair is close enough to the table (meaning that noone is sitting there).
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-14.png)

### 15. The display should be turned back on when the chair is far enough from the table.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-15.png)

### 16. One of the children of this GameObject is NUIX Speech recognition. I decided to not make it complex, so you have more freedom in developing your own specific speech recognition logic. However, if you just want to perform actions by special keywords, this recognizer should be enough. For each type of action, create a GameObject with a wordAction component attached to it. Drag each of the wordAction gameobjects to the trigger words elements.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-16.png)

### 17. In this example, when a student wants to ask a question, he usually pronounces the "Question" word. Once the student said "Teacher, I have a question", the sentence is parsed by words and each of the words is compared to the words you set to trigger an action, which is turning on the camera on the desk. After the student heard an answer for the question, he usually says "Thank you teacher / Thanks / etc". For example, when "Thanks" is pronounced, camera recording is turned off.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-17.png)

### 18. To test the project, go the File-Build Settings, check if the scene is in the build, if Oculus Device is selected and press build and run.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-18.png)

### 19. Moving the chair closer to the table turns off the screen.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-19.png)

### 20. The Thanks word is recognized and camera stops recording.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-20.png)

### 21. To save your device, create a folder for it in the NUIX-Studio SDK.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-21.png)

### 22. Next, drag your device GameObject into the project window. 
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-22.png)

### 23. Now you have created a .prefab file for the smart device, which you can share to your team members.
![](https://github.com/FedorIvachev/IoThingsLab-ReadmeFiles/blob/master/Tutorials/NUIX-Tutorial-CreateDevice-Pictures/NUIX-Tutorial-CreateDevice-23.png)

## In the next tutorial you will know about each of the items for creating IoT devices NUIX studio provides.
