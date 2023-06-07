# Frontend tasks

Simple tasks to gain some familiarity with the main APIs and a chance to show off some of your skills.  
Time expectations: < 3 hours.

Create your own public repo that you can share with us when you've finished.
Try to structure the code as you would in a production app rather than a PoC.  
Prioritize finishing the tasks over designing a neat looking UI.  
Write TS or JS code. We prefer TS if you already know the language.  
Use React if you feel comfortable, or any other libraries if you prefer. 

## 1. Load scene

Load the condos scene with ID `3b5e65560dc4422da5c7c3f827b6a77c`.  
The canvas should take up the entire width and height of the browser window.  
The view's camera controller should be a `"flight"` controller.

Links:
- [DEMO - Getting started](https://docs.novorender.com/docs/tutorials/getting_started)
- [DEMO - Loading scenes](https://docs.novorender.com/docs/tutorials/loading_scenes)
- [DOCS - createCameraController()](https://docs.novorender.com/docs/webgl-api/interfaces/NovoRender.API#createcameracontroller)

## 2. Store camera positions

Create 3 buttons on top of the Canvas.  
They do not need to look pretty.  
Each button should work like this: 

- `Shift + Left click`: Save current camera position and rotation.
- `Left click`: Go to the stored position and rotation.

You should then be able to move around the 3D scene and save up to 3 positions that you can jump back to.

Links:
- [DOCS - Camera position](https://docs.novorender.com/docs/webgl-api/interfaces/NovoRender.Camera#position)
- [DOCS - Camera rotation](https://docs.novorender.com/docs/webgl-api/interfaces/NovoRender.Camera#rotation)
- [DOCS - Camera moveTo()](https://docs.novorender.com/docs/webgl-api/interfaces/NovoRender.CameraController#moveto)

## 3. Isolate objects  

Create a form with a single text input element together with a submit button on top of the Canvas.  
No need to make these elements pretty either.  
The form should work like this:  
- Search the scene for objects containing the input string.
- If any results (e.g. search for `"chair"`):
    - Hide all other objects.
    - Show only the results in their neutral colours. 
- If no result (e.g search for `"choir"`):
    - Show all objects in their neutral colours.
- Abort currently running search if a new one is starting.  

Links:
- [DEMO - Searching](https://docs.novorender.com/docs/tutorials/searching)
- [DOCS - Search](https://docs.novorender.com/docs/webgl-api/interfaces/NovoRender.Scene#search)
- [DEMO - Object highlighting](https://docs.novorender.com/docs/tutorials/object_selection#object-highlighting)
- [DOCS - createHighlight()](https://docs.novorender.com/docs/webgl-api/interfaces/NovoRender.API#createhighlight)
- [DOCS - NeutralHighlightParams](https://docs.novorender.com/docs/webgl-api/interfaces/NovoRender.NeutralHighlightParams)
