#Add Aframe interactions
1. Raycasting- Add cursor="rayOrigin:mouse;"
   Eg: <a-scene cursor="rayOrigin:mouse;">
2. Using the camera for raycasting
   In aframe, a camera is given by default if it is not specified and is placed at a height of
   from the ground. When we are trying to render a 3D scene, we have to specify what is actually looking in the scene, that is what is called a virtual CAMERA. That camera can be added in an entity
   <a-entity id="stand">
   <a-entity camera position="0 2 0" look-controls wasd-controls>
   <a-cursor id="cursor" raycaster fuse="true" fusetimeout="3000"></a-cursor>
   </a-entity>
   </a-entity>