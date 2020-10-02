# Brighan Schwind- VR project 1- ID#12

My project is simply a mirrored version of my apartments room between before covid and after covid.

## BEFORE

![Before Covid](https://github.com/BrighanSchwind/Project1/blob/master/Project1ScreenShots/BeforeCovid.JPG)

## AFTER

![After Covid](https://github.com/BrighanSchwind/Project1/blob/master/Project1ScreenShots/AfterCovid.JPG)

### There are 3 things that the user can do within my project.
2 of them are if you click the pillow farthest from the wall it will move you into the mirrored room with the lighting being toggled.

![Bed](https://github.com/BrighanSchwind/Project1/blob/master/Project1ScreenShots/Bed.JPG)

```
<!--User-->
     <a-entity id="camera" camera="userHeight: 1.6" universal-controls cursor="rayOrigin: mouse" position = "73 1.5 -16"></a-entity>
<!--ClickableObjects-->
  <a-box position="45 1 -18" rotation="0 0 0" color="#000" shadow
             onclick="MoveToNoCovid()"></a-box>
	<a-box position="74 1 -18" rotation="0 0 0" color="#000" shadow
             onclick="MoveToCovid()"></a-box>
```

```
function MoveToCovid(){
    document.getElementById('camera').setAttribute('position', '48 3 -16')
     document.getElementById('light').setAttribute('visible', 'true');
    document.getElementById('light2').setAttribute('visible', 'false');
  }
  function MoveToNoCovid(){
    document.getElementById('camera').setAttribute('position', '73 3 -16')
     document.getElementById('light').setAttribute('visible', 'false');
    document.getElementById('light2').setAttribute('visible', 'true');
  }
```
The last being that if the lights are off you can turn them on by clicking the light switch

![LightSwitch](https://github.com/BrighanSchwind/Project1/blob/master/Project1ScreenShots/LightSwitch.JPG)

```
<!--User-->
     <a-entity id="camera" camera="userHeight: 1.6" universal-controls cursor="rayOrigin: mouse" position = "73 1.5 -16"></a-entity>
<!--ClickableObjects-->
<a-box position="60 3 -2" rotation="0 0 0" color="#000" scale = "1.1 .5 .5" shadow
            onclick="TurnLights()"
         ></a-box>
```

```
function TurnLights() {
   
    document.getElementById('light').setAttribute('visible', 'true');
    document.getElementById('light2').setAttribute('visible', 'false');
    
    
    }
```
# Finaly the ceiling fan moves

![fan](https://github.com/BrighanSchwind/Project1/blob/master/Project1ScreenShots/CeilingFan.JPG)

```
<!-- Fan-->
   <a-obj-model src="assets/fan.obj" mtl="assets/fan.mtl" position="70 9.5 -10" rotation="0 0 0"  scale = ".05 .05 .05">
   <a-animation attribute="rotation"
                     easing="linear"
                     dur="10000"
                     to="0 360 0"
                     repeat="indefinite">

        </a-animation></a-obj-model>
```

# Resources:
Couch: https://www.cgtrader.com/items/190535/download-page

Desk: https://www.cgtrader.com/items/712176/download-page

Chair: https://www.cgtrader.com/items/1938755/download-page

Lamp: https://www.cgtrader.com/items/1996923/download-page

Trash Can: https://www.cgtrader.com/items/1933717/download-page

Window: https://www.cgtrader.com/items/244717/download-page

TV: https://www.cgtrader.com/free-3d-models/electronics/video/sony-bravia-kdl-42-w655a-smart-led-tv-42-39f53412db8c27b537f84359d62b75aa

Monitor: https://www.cgtrader.com/items/2077440/download-page

Computer:https://www.cgtrader.com/items/244717/download-page

Bed: https://www.cgtrader.com/items/640956/download-page

Mouse: https://www.cgtrader.com/items/2518304/download-page

Drawer: https://www.cgtrader.com/items/2075808/download-page

Keyboard: https://www.cgtrader.com/items/203984/download-page

Book: https://www.cgtrader.com/items/313466/download-page

Fan:https://www.cgtrader.com/items/199620/download-page

Images
Night: https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.discovery.com%2Fscience%2Fstuck-at-home--try-looking-up-&psig=AOvVaw18MRhFVXTNGgWFmFxM2pvr&ust=1601496880065000&source=images&cd=vfe&ved=0CA0QjhxqFwoTCPDk_ISXj-wCFQAAAAAdAAAAABAD

Sky:
https://www.google.com/url?sa=i&url=https%3A%2F%2Fcommons.wikimedia.org%2Fwiki%2FFile%3ASky.jpg&psig=AOvVaw3f1_4p0scyC3VdZLaYJ1Bi&ust=1601503150035000&source=images&cd=vfe&ved=0CA0QjhxqFwoTCOict62uj-wCFQAAAAAdAAAAABAD

VideoLink : https://youtu.be/ttHvILn5nZ0
Website:https://brighanschwind.github.io/Project1/
SourceCode:https://github.com/BrighanSchwind/Project1/blob/master/index.html
