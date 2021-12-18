# NUIX-Studio SDK - Devices

Selected action - inside unity editor, press on the plus button, then drag a GamObject into the empty field or choose it from the list, select a method attached to one of this GameObjects Components to be performed.

## Basic Interactables

Type | Description | Located at
------------ | ------------- | ------------
Audio | GameObject with an Audio Source Component | SDK/UX/Interactables/Prefabs/Audio/Audio.prefab
Camera | GameObject with a Camera Component, writing the data into CameraRenderTexture | SDK/UX/Interactables/Prefabs/Camera/Camera.prefab
Camera Render Texture | A render texture to store the Camera Image Data | SDK/UX/Interactables/Textures/CameraRenderTexture.renderTexture
Camera Render Texture Material | A material to store the Camera Render Texture | SDK/UX/Interactables/Materials/CameraRenderTextureMaterial.mat
Display | A Plane GameObject with a Camera Render Texture applied to it | SDK/UX/Interactables/Prefabs/Camera/Display.prefab
Light | A GameObject with Light Component | SDK/UX/Interactables/Prefabs/Light/Light.prefab
Video | A Plane GameObject with Video Player Component | SDK/UX/Interactables/Prefabs/Video/Video.prefab

## Basic Sensors

Type | Description | Located at
------------ | ------------- | ------------
Contact | Two movable square cuboids with a contact sensor: when a distance between them exceeds the defined value, a selected action is performed  | SDK/UX/Prefabs/ContactSensor/Contact.prefab
GestureFist, GestureSpiderMan, GestureThumbsUp | Examples of gesture sensors; when triggered, a selected action is performed | SDK/UX/Prefabs/Gestures
SightSensor | When a selected Target GameObject Appears at the selected Camera View, a selected action is performed | SDK/UX/Prefabs/SightSensor/SightSensor.prefab
SpeechRecognition | When a defined word is said, an action is performed. You need to connect to Wi-Fi to use it | SDK/UX/Prefabs/Speech/SpeechRecognition.prefab
WeightSensor | A Plane GameObject; when the total weight of GameObject lying/intersecting it exceeds the defined weight, a selected action is performed | SDK/UX/Prefabs/WeightSensor/WeightSensor.prefab
