# With Three JS

<img src="https://resources.gdevelop-app.com/assets/Icons/rotate-3d.svg" class="extension-icon"></img>
Create a simple 3D scene.

**Authors and contributors** to this community extension: [PANDAKO](https://gd.games/PANDAKO).

!!! warning
    This is an extension made by a community member — but not reviewed
    by the GDevelop extension team. As such, we can't guarantee it
    meets all the quality standards of official extensions. In case of
    doubt, contact the author to know more about what the extension
    does or inspect its content before using it.

---

Extension for GDevelop to create simple 3D scenes.  
This extension is intended for easy and simple 3D rendering. It does not currently aim for realistic rendering with light and shadow.  

## ⚠️ Precautions for use  
This extension is experimental. Destructive changes may be made.  

## 📖 How to use  
Check out this page.  
[WithThreeJs Extension for GDevelop](https://pandako.itch.io/with-threejs-extension-for-gdevelop)  

## 🍩 Donation  
Currently, I'm doing development in between jobs, but if many people support me, I will be able to devote more time to the development.  
If you enjoy this extension, please consider [downloading the Example project file](https://pandako.itch.io/with-threejs-extension-for-gdevelop) to maintain this extension. (The Example project file will surely help you.😉)  

## Three.js  
Copyright 2010-2022 Three.js Authors  
https://github.com/mrdoob/three.js/blob/dev/LICENSE

[Read more...](https://pandako.itch.io/with-threejs-extension-for-gdevelop)

!!! tip
    Learn [how to install new extensions](/gdevelop5/extensions/search) by following a step-by-step guide.

## Actions

**Add Child**  
Add 3D Object as child to 3D object.

**Built-In 3D WithThreeJS (Ultra Super Experimental)**  
Use this action in place of the "Create 3D Scene" action.  
The built-in 3D axes are different from the axes in WithThreeJS.
Some WithThreeJS features are not available.
⚠️ This may be deprecated in the future.

**3D Camera Look At 3D Object**  
3D Camera Look At 3D Object

**Change 3D Camera FOV**  
Change the Field Of View of the 3D Camera.

**Change 3D Camera Far**  
Change the far property of 3D Camera.  
The 3D Camera will not render 3D Objects farther than this distance.

**Change 3D Camera Near**  
Change the near property of the 3D Camera.  
The 3D Camera will not render 3D Objects closer than this distance.

**Change 3D Camera Zoom**  
Change 3D Camera Zoom

**Change 3D Texture**  
Change the 3D Texture of a 3D Object.

**Change 3D Object All Animations Speed Scale**  
Change all animations speed scale of a 3D Object.  
0 is pause.
Negative values play backwards.

**Change 3D Object DepthWrite (Experimental)**  
Change the DepthWrite of a 3D Object.  
Whether rendering this 3D Object has any effect on the depth buffer.
If transparent 3D Objects overlap and render incorrectly, you may be able to obtain ideal rendering results by setting the DepthWrite of that 3D Object to No.
Default is Yes.

**Change Master Volume Of 3D Scene**  
Change Master Volume Of 3D Scene

**Change 3D Object Opacity**  
Change the Opacity of a 3D Object.  
The same value is set for multiple textures.

**Change 3D Object Scale**  
Change the Scale of a 3D Object.  
Note that 3D Sprite and 3D Model were scaled when created.

**Change 3D Object Visibility**  
Change the visibility of a 3D Object.

**Clear 3D Scene**  
Clear 3D Scene. Removes all 3D Objects in the 3D Scene.  
As a result, this action also removes 2D Objects that have 3D Projection Behaviors.
This action does not clear the loaded 3D Texture data and the loaded 3D Model data.
They will continue to be accessible by ID.

**Correct 3D Camera Rotation Within Limits (Deprecated)**  
Correct the 3D Camera Rotation within limits.  
Rotation is corrected like head movement. Limiting multiple axes can break things.

**Correct 3D Object Rotation Within Limits (Deprecated)**  
Correct the 3D Object Rotation within limits.  
Using this action on a 3D Object rotated on multiple axes may not work correctly.

**Create 3D Axes Helper**  
Create 3D Axes Helper

**Create 3D Box**  
Create 3D Box

**Create 3D Model**  
Create 3D Model

**Create 3D Model From Built-In 3D Model**  
Create 3D Model From Built-In 3D Model

**Create 3D Plane**  
Create 3D Plane

**Create 3D Scene**  
Create a 3D Scene and initialize all 3D Cameras.

**Create 3D Sprite**  
Create 3D Sprite

**Detach From Parent**  
Detach a 3D Object from its parent.  
(Set Parent to Scene)

**Load 3D Model From OBJ**  
Load 3D Model From OBJ

**Load 3D Texture**  
Load image from GDevelop resources and create 3D Texture.

**Look At 3D Camera**  
Look At 3D Camera

**Look At 3D Object**  
Look At 3D Object

**Move 3D Camera**  
Move a 3D Camera.  
'=' is relative to the parent axis.
"+" and "-" are relative to the local axis.

**Move 3D Object**  
Move a 3D Object.  
'=' is relative to the parent axis.
"+" and "-" are relative to the local axis.

**Move 3D Object On World**  
Move a 3D Object on the world axis.  
"=", "+" and "-" are relative to the world axis.

**Output All IDs To Console**  
Output All IDs To Console

**Output 3D Model Information To Console**  
Output 3D Model Information To Console

**Play 3D Animation**  
Play 3D animation.  
If already playing, only the "Animation Speed Scale" and "Loop" parameters are updated.

**Play 3D Sound**  
Play a 3D Positional Sound.

**Raycast**  
Do a Raycast.  
You can get the count of 3D Objects in the result with the "Raycast Result Count" expression.
The result can be accessed via the "Raycast Result Number" expression or the "Raycast Result String" string expression.

**Raycast From 3D Camera**  
Do a Raycast from the 3D Camera.  
You can get the count of 3D Objects in the result with the "Raycast Result Count" expression.
The result can be accessed via the "Raycast Result Number" expression or the "Raycast Result String" string expression.

**Remove 3D Object**  
Remove a 3D Object from the 3D Scene.  
This action cannot remove 3D Objects created by 3D Projection Behaviors.
This action does not clear the loaded 3D Texture data and the loaded 3D Model data.
They will continue to be accessible by ID.

**Resolve Bounding Box Collision**  
Resolve collisions between Bounding Boxes.  
It is not necessary to use the "Check Bounding Box Collision" condition beforehand. (It will do almost the same processing)
Note that the 3D Objects are still in contact after resolution. ("Check Bounding Box Collision" condition will not be false.)
3D Object thickness too thin for the amount of movement will not resolve correctly.
This action updates the "Bounding Box Collision Result".

**Rotate 3D Camera**  
Rotate the 3D Camera in the order X, Y, Z.

**Rotate 3D Camera Like Head**  
Rotate the 3D Camera first in the world Y axis, then on the local X and Z axes.

**Rotate 3D Camera On World**  
Rotate the 3D Camera in the order X, Y, Z on the world axis.

**Rotate 3D Object**  
Rotate the 3D Object in the order X, Y, Z.

**Rotate 3D Object Like Head**  
Rotate the 3D Object first in the world Y axis, then on the local X and Z axes.

**Rotate 3D Object On World**  
Rotate the 3D Object in the order X, Y, Z on the world axis.

**Set 3D Object ID Of Children To Scene Variable**  
Set 3D Object ID of all children to scene variable as array.

**Setup Multiple 3D Cameras**  
Note that rendering time increases by the number of enabled 3D Cameras.

**Stop 3D Animation**  
Stop 3D Animation

**Stop 3D Sound**  
Stop a 3D Positional Sound.

**Update Bounding Box Helper**  
Create or update Helper to graphically display Bounding Box.

## Conditions

**Check 3D Animation Is Finished**  
Check if the 3D Animation is finished.  
This condition is valid only for animations with "Loop" set to "Once".

**Check 3D Animation Is Playing**  
Check if the 3D Animation is playing.

**Check 3D Sound Is Playing**  
Check if the 3D Sound is playing.

**Check Bounding Box Collision**  
Checks for collisions between the Bounding Boxes of two 3D Objects.  
This condition updates the "Bounding Box Collision Result" when it returns True.

**Check Existence Of 3D Object**  
Check Existence Of 3D Object

**Check Visibility Of 3D Object**  
Check the visibility of a 3D Object.  
This condition cannot be tested correctly if the visibility of the 3D object is changed by inheritance.

## Expressions

| Expression | Description |  |
|-----|-----|-----|
| `WithThreeJS::BoundingBoxCollisionResultNumber(string)` | Bounding Box Collision Result Number ||
| | _string_ | Item |
| `WithThreeJS::CameraAngle(number, string)` | 3D Camera Angle for GDevelop.Returns the angle of an individual axis.Note that combining the resulting XYZ values may not reproduce the original rotation. ||
| | _number_ | 3D Camera ID (1 to 4) |
| | _string_ | Axis |
| `WithThreeJS::CameraDirection(number, string)` | Normalized direction vector of 3D camera.(3D Camera is shooting in the negative Z axis direction) ||
| | _number_ | 3D Camera ID (1 to 4) |
| | _string_ | Axis |
| `WithThreeJS::CameraFOV(number)` | 3D Camera FOV ||
| | _number_ | 3D Camera ID (1 to 4) |
| `WithThreeJS::CameraFar(number)` | 3D Camera Far ||
| | _number_ | 3D Camera ID (1 to 4) |
| `WithThreeJS::CameraNear(number)` | The camera will not render objects closer than this distance. ||
| | _number_ | 3D Camera ID (1 to 4) |
| `WithThreeJS::CameraPosition(number, string)` | 3D Camera Position ||
| | _number_ | 3D Camera ID (1 to 4) |
| | _string_ | Axis |
| `WithThreeJS::CameraRotation(number, string)` | 3D Camera Rotation ||
| | _number_ | 3D Camera ID (1 to 4) |
| | _string_ | Axis |
| `WithThreeJS::CameraZoom(number)` | 3D Camera Zoom ||
| | _number_ | 3D Camera ID (1 to 4) |
| `WithThreeJS::DistanceFrom3DCameraTo3DObject(number, identifier)` | Distance From 3D Camera To 3D Object ||
| | _number_ | From 3D Camera ID (1 to 4) |
| | _identifier_ | To 3D Object ID |
| `WithThreeJS::DistanceFrom3DObjectTo3DObject(identifier, identifier)` | Distance From 3D Object To 3D Object ||
| | _identifier_ | From 3D Object ID |
| | _identifier_ | To 3D Object ID |
| `WithThreeJS::MasterVolumeOf3DScene()` | Master Volume Of 3D Scene ||
| `WithThreeJS::ObjectAnimationDuration(identifier, number)` | 3D Object Animation Duration ||
| | _identifier_ | 3D Object ID |
| | _number_ | Original Animation Number |
| `WithThreeJS::ObjectAnimationSpeedScale(identifier, number)` | 3D Object Animation Speed Scale ||
| | _identifier_ | 3D Object ID |
| | _number_ | Original Animation Number |
| `WithThreeJS::ObjectAnimationTime(identifier, number)` | 3D Object Animation Time ||
| | _identifier_ | 3D Object ID |
| | _number_ | Original Animation Number |
| `WithThreeJS::ObjectDirection(identifier, string)` | Normalized direction vector of 3D Object.(Z axis direction) ||
| | _identifier_ | 3D Object ID |
| | _string_ | Axis |
| `WithThreeJS::ObjectOpacity(identifier)` | 3D Object Opacity ||
| | _identifier_ | 3D Object ID |
| `WithThreeJS::ObjectParent(identifier)` | 3D Object Parent ||
| | _identifier_ | 3D Object ID |
| `WithThreeJS::ObjectPosition(identifier, string)` | 3D Object Position ||
| | _identifier_ | 3D Object ID |
| | _string_ | Axis |
| `WithThreeJS::ObjectPositionOnWorld(identifier, string)` | 3D Object Position On World ||
| | _identifier_ | 3D Object ID |
| | _string_ | Axis |
| `WithThreeJS::ObjectRotation(identifier, string)` | 3D Object Rotation ||
| | _identifier_ | 3D Object ID |
| | _string_ | Axis |
| `WithThreeJS::ObjectRotationOnWorld(identifier, string)` | 3D Object Rotation On World ||
| | _identifier_ | 3D Object ID |
| | _string_ | Axis |
| `WithThreeJS::ObjectScale(identifier, string)` | 3D Object Scale ||
| | _identifier_ | 3D Object ID |
| | _string_ | Axis |
| `WithThreeJS::PointOf3DObjectOn3DCamera(number, identifier, string)` | Point Of 3D Object On 3D Camera ||
| | _number_ | 3D Camera ID (1 to 4) |
| | _identifier_ | 3D Object ID |
| | _string_ | Axis Of Return Value |
| `WithThreeJS::PointOfPositionOn3DCamera(number, number, number, number, string)` | Point Of World Position On 3D Camera ||
| | _number_ | 3D Camera ID (1 to 4) |
| | _number_ | World Position X |
| | _number_ | World Position Y |
| | _number_ | World Position Z |
| | _string_ | Axis Of Return Value |
| `WithThreeJS::RaycastResultCount()` | Count of 3D Objects in Raycast Result ||
| `WithThreeJS::RaycastResultNumber(number, string)` | Raycast Result Number ||
| | _number_ | Index (0 or more) |
| | _string_ | Item |
| `WithThreeJS::RaycastResultString(number, string)` | Raycast Result String ||
| | _number_ | Index (0 or more) |
| | _string_ | Item |

## 3D Box (Experimental) 

This 3D Box can have different textures on 6 faces.
⚠️ This object is high load. 

### Object expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.Depth()` | Depth ||
| `Object.Id()` | 3D Object ID ||

## 3D Board Projection 

Create 3D Board (Plane) from Sprite object. Moving that Sprite will also move the 3D Object. 

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.BoardProjection::AlphaTest()` | Alpha Channel Test ||
| `Object.BoardProjection::AngleAxis()` | Axis linked to 2D Object Angle ||
| `Object.BoardProjection::Id()` | 3D Object ID ||
| `Object.BoardProjection::Orientation()` | Orientation ||

## 3D Box Projection from Tiled Sprite 

Create 3D Box from Tiled Sprite object. Moving that Tiled Sprite will also move the 3D Object. 

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.BoxProjectionFromTiled::AlphaTest()` | Alpha Channel Test ||
| `Object.BoxProjectionFromTiled::Blend()` | Blend Mode ||
| `Object.BoxProjectionFromTiled::Depth()` | Depth ||
| `Object.BoxProjectionFromTiled::Id()` | 3D Object ID ||

## Linked 3D Camera 

Link a Sprite object and  a 3D Camera. 

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.LinkedCamera::Fov()` | Field Of View ||
| `Object.LinkedCamera::Id()` | 3D Camera ID ||

## 3D Model Transfer (Deprecated) 

🚫 The recommendation is to use the "Create 3D Model From Built-In 3D Model" action instead of this behavior.
This behavior transfers the built-in 3D model to the WithThreeJS 3D Scene.
The original 2D object is deleted.
⚠️ This may be deprecated in the future. 

_No expressions for this behavior._


## 3D Plane Projection from Tiled Sprite 

Create 3D Plane from Tiled Sprite object. Moving that Tiled Sprite will also move the 3D Object. 

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.PlaneProjectionFromTiled::AlphaTest()` | Alpha Channel Test ||
| `Object.PlaneProjectionFromTiled::Blend()` | Blend Mode ||
| `Object.PlaneProjectionFromTiled::Id()` | 3D Object ID ||

## 3D Sprite Projection 

Create 3D Sprite from Sprite object. Moving that Sprite will also move the 3D Sprite. 

### Behavior expressions

| Expression | Description |  |
|-----|-----|-----|
| `Object.SpriteProjection::AlphaTest()` | Alpha Channel Test ||
| `Object.SpriteProjection::Id()` | 3D Object ID ||

---

*This page is an auto-generated reference page about the **With Three JS** extension, made by the community of [GDevelop, the open-source, cross-platform game engine designed for everyone](https://gdevelop.io/).* Learn more about [all GDevelop community-made extensions here](/gdevelop5/extensions).