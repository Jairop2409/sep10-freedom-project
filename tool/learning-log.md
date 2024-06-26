# Tool Learning Log

Tool: **Aframe**

---

3/3/24:
* watched a video about position using Aframe _*[Youtube video](https://www.youtube.com/watch?v%253DliOLtcPmMa0)_*
* read the documentation of positioning on  the Aframe [page](https://aframe.io/docs/1.5.0/components/position.html)
 ##### Things I changed  using the video
- I used aspect ratio to change the width, height, and depth of a shape, I made the `height="0.1"`, `Width="2"` `position=" 1, 0.75,-2`
 ![practice](<images/Aspectratio .png>)
 #### Things made
 - Using the aframe page and using the code I made a cylinder stack upon the first cylinder, I changed the color and I created a cone on top of both cylinders
 * The code That I used for creating a cone was
 `
 <a-cone
        position=" 1 1.5 -2"
        radius="0.5"
        height="0.5"
        color="#0000FF"
        width= "8"
        depth="1.2"
      ></a-cone>

* The code I used for creating a cylinder was
`
 <a-cylinder
     position=" 1 1 -2"
     radius="0.5"
    height="0.5"
    color="#0000FF"
    width= "8"
    depth="1.2"
     ></a-cylinder>
#### End product
![What I made](<images/Product.png>)

### Challenges
* The challenge I faced when trying to make new shapes using positions, width, and height was making sure it was the way I wanted and making sure the shapes/Entity had the right position( on top of the cylinder/s) I found making everything the way I wanted difficult but using the video tutorial and the Aframe webpage I was able to found out what was x,y and z in the
`a-entity position="x y z"></a-entity>
` code

### Questions
Is it possible to make an entity inside an entity code?> for example `a-circle` inside the code for `a-clyinder`?

### Next steps
* Try other components and their meaning and how I can use them on my fp(freedom) project

3/9/24:

* **Watched 15 minutes about creating Geometry objects and changing colors,width,height ect on an object  [Youtube video](https://www.youtube.com/watch?v%253DnRK6-FKobis)**
* read the documentation of Geometry(objects) on  the Aframe [page](https://aframe.io/docs/1.5.0/components/geometry.html)



##### Things I changed using both the documentation and video
* I changed the sky color to a crystal blue color. The code I used was
` <a-sky color=#5CB3FF></a-sky> `.
* I created a geometry object(ring) and I Made it have a color of red and changed the `radius:inner` and `Radius:outter`.
* The code I used was

 `<a-ring geometry="primitive: ring; radiusInner: 4; radiusOuter: 10"
          material="side: double" color="red"></a-ring>
    `
   ![Ring](images/Ring.png)

#### Things I made
* I changed the plane position to go inside the ring
* The code I used for this was
` <a-plane position="0 1-4" rotation="-90 0 0" width="4" height="4" color="#7BC8A4"></a-plane>
`
* I modified the ring to have a position and created 2 other rings. I made a ring with a blue color and another one with green. Finally, I tested out the position and see if it lined up the way I wanted and it did.
* The code I  used was

`
 <a-ring geometry="primitive: ring; radiusInner: 4; radiusOuter: 11"
          material="side: double" color="Red" position="1 0.75 -0.045" ></a-ring>
       <a-ring geometry="primitive: ring; radiusInner: 4; radiusOuter: 11"
          material="side: double" color="Blue" position="1 0.75 -0.025"></a-ring>
     <a-ring geometry="primitive: ring; radiusInner: 4; radiusOuter: 11"
          material="side: double" color="green" position="1 0.75 -0.035"></a-ring>
    `
* Final product
![Ringrainbow](images/Geometryrainbow.png)
### Challenges
The challenge I faced  was when  I placed an object because I had to make it the way I wanted. I wanted it to line up but whenever I created a new ring it Overlapsed with the first ring so I had to change the Position. After looking back at Aframe and the way I did it before, it helped me change where the ring went and how it was placed.
### Questions
How can I use a 360 image as an image? like for example if I wanted the `<a-sky>` to be a picture instead of a color

## What I plan to do next
* _Study one more component_
___
3/16/24:

Some things I did to practice the components of aframe were
*  practiced what I learned for the past weeks and tried to make something using what I learned
* The new component I learned was light and I read a documetation about it [light](https://aframe.io/docs/1.5.0/components/light.html#adding-real-time-shadows)

##### Things I made  from reading the documentation
*  I tried to make a `point` light which is basically a light that affects materials based on where they are located in
* The  code I used for this was
```
  <a-entity light="type: point; intensity: 5  distance: 0; decay: 0"
          position="1 0.75 1.75"></a-entity>
```
and I added a shadow to the image to make the scene less dark
* The code I used was
```
   <a-scene shadow="type: pcfsoft">


</a-scene>
```
### end product
![image](images/light.png)

## Practicing what I learned
 Some things I made were
*  a geometry shape called "octahedron"
   * The code I used for this was ` <a-octahedron position="-2.5 0.5 0.5" color="red" radius="0.45"></a-octahedron>`
*  made a triangle
   * The code I used for this was
   ```
    <a-entity geometry="primitive: triangle" material="side: double" color="Blue" position="1 3 -3"></a-entity>
   <a-entity geometry="primitive: triangle" material="side: double" color="Blue" position=".5 2 -3"></a-entity>
    <a-entity geometry="primitive: triangle" material="side: double"color="Blue" position="1.5 2 -3"></a-entity

      ```
Made three triangles facing each other
* The last thing I made was a shape called " Torus"
   * The code I used for this was
```
      <a-entity geometry="primitive: torus; radius: 5; radiusTubular: .5; arc: 360" color="Red" position="0.025 0.75 -0.045"></a-entity>
```
The things I changed was made the radius bigger(the inside)


### Final product
![geometry](images/Practice.png)
#### Challenges
One challenge I faced was the light part because It showed a shadow on top of the three shapes and when I added the shadow code, it no longer had a shadow. Another challenge I faced was deciding which component to do because some require animation and I haven't done that yet.
#### Questions
* Is there a way to make my shape's have a color because there was an error. One example is ` <a-octahedron`
### *what I plan to do next*
* Learning animation and/or  cursor
___
3/22/24:
* Watched a 15 minute video on  learning animation **[youtube aframe video](https://www.youtube.com/watch?v=p3mNNZ356Ko)**
    * Website from Video [Animation](https://matthewlein.com/tools/ceaser)
*  read the documentation of Animation on  the Aframe [page](https://aframe.io/docs/1.5.0/components/animation.html)

##### Things I changed using the video and the documentation
* When I read the animation page I read that  animations are a component where you change a object value and their appearance
    * what  I changed was the position of where the shape started
![Ringrainbow](images/Animation.png)
* The code I used was  `
   <a-box position="-4 1.6 -5" animation="property: position; to: 1 8 -10; dur: 2000; easing: linear; loop: true" color="tomato"></a-box>
   `

#### What I learned from the video
- setting an attribute to an animation can set the animation to autoplay

#### What I made and how I used  Previous things I learned to add to what I learned
* I made   1 box and another animated box
  * The code I used for making another animated box was

   `<a-box position="1 0.75 -3" animation="property: position; to: 1 8 -10; dur: 2000; easing: linear; loop: true" color="blue"></a-box>
   `
   * The code I used for making a box was
   ` <a-entity geometry="primitive: box;   width: 1; height: 1; depth: 1"; position=" 1 1.75 -3"></a-entity>`
#### Final product
![box](images/box.png)

### Challenges
*  One challenge I faced was understanding how animations worked because I found the  different types of easing hard because they animate different things
      * Example: scaling
### Questions
* Is there a way to scale while an object is in motion?
### What I plan to do next
*  Learn cursor and/ or  camera
___
3/31/24
* Learned how to use cursor in the aframe [page](https://aframe.io/docs/1.5.0/components/cursor.html) and I used the raycaster [page](https://aframe.io/docs/1.5.0/components/raycaster.html) to see the cursor in actions.

Before I explain what I changed, and made and my progress, we need to know what a cursor is and a raycaster.
* What is a Cursor?
   * A cursor is a hover component that has  a camera built to see control base interactions.
* What is a raycaster?
   * A raycaster is checking for events and the intersections that cross it
#### Things I changed
* One thing I changed was the color of the cursor  and Positioning the cursor to the raycaster
    * The code I used was
    `
<a-entity camera look-controls>
  <a-entity cursor="fuse: true; fuseTimeout: 500"
            position="0 0 -1"
            geometry="primitive: ring; radiusInner: 0.02; radiusOuter: 0.03"
            material="color: red; shader: flat">
  </a-entity>
  `

As you see `material="color: red; ` means the camera cursor turns red.

* Another thing I changed was making the raycastor have an animation
     * The code for making a raycaster
    `<a-entity id="player" >
  <a-entity collider-check raycaster="objects: .collidable; showLine:true;" position="1 1 1"></a-entity>
</a-entity>
`

This made a raycastor and what I changed is making it move as an animation using the code
* `<a-entity class="collidable" geometry="primitive: box"  position="0 1 -3"  animation="property: position; to: 1 8 -10; dur: 2000; easing: linear; loop: true" color="blue"></a-entity>
`
##### Takeaways for cursor
Using what I learned from animations I added onto with cursor and raycaster's
##### Final product
![hey](images/Cursor.png)

#### Things I made
* I made a red cylinder in raycastor
* I made another animated box
     * Code used
     `<a-entity class="collidable" geometry="primitive: box"  position="3 1 -3"  animation="property: position; to: 1 0 -5; dur: 1000; easing: linear; loop: true" color="blue"></a-entity>
`

My final product
![final product](images/Finalproduct.png)

### Challenges
* A challenge I faced was doing cursors because it was hard to understand where everything had to be positioned because when adding the raycaster it caused the camera to face the raycaster

### Questions
* How can I prepare for next week?

## My plans for the upcoming weeks
* Next week-  building a basic scene
* In two weeks...
     * Building a 360
    * Extension-
        * Practicing everything I learned in my ide instead of js bin
* tbd
___


4/10/24
* Read a Documentation about [sound](https://aframe.io/docs/1.5.0/components/sound.html) and practiced for three days in my IDE to use what I learned about Animation and their easing to expand my animations.

#### Things  I changed
* Sound-
   * When I read the documentation from sound I learned a couple things
       * One thing I learned is in order to use this component you must create your own audio and sound and upload it.
       * Another way is if you look for audio and upload it by downloading the sound
   * The code I used was

  <a-scene>

        <a-assets>
            <audio id="river" src="river-6.mp3" preload="auto"></audio>
          </a-assets>

          <a-entity sound="src: #river"></a-entity>


        <a-box position="-1 0.5 -3" rotation="0 45 0" color="#4CC3D9"></a-box>
        <a-sphere position="0 1.25 -5" radius="1.25" color="#EF2D5E"></a-sphere>
        <a-cylinder
          position="1 0.75 -3"
          radius="0.5"
          height="1.5"
          color="#FFC65D"
          id="river"
         sound="src https://www.soundjay.com/nature/sounds(river-6.mp3); autoplay: true;">
        </a-cylinder>
         <a-plane
          position="0 0 -4"
          rotation="-90 0 0"
          width="4"
          height="4"
          color="#7BC8A4"
        ></a-plane>
        <a-box position="1 0.75 -3" scale="1.5 1 2" animation="property: position; to: -3 8 -10; dur: 1100; easing: linear; loop: true" color="blue"></a-box>
        <a-box position="1 0.75 -3" animation="property: position; to: 1 8 -10; dur: 1000; easing: linear; loop: true" color="red"></a-box>
        <a-entity geometry="primitive: box;   width: 1; height: 1; depth: 1"; position=" 1 1.75 -3"></a-entity>
        </a-sky>
        </a-scene>
* Some things I changed was the music and  made  the music go in the cylinder

##### Things I  made
* Animation
     * One thing I made was that I made a sphere and made it orbit around a  box.
* The code I used for this was
`<a-entity rotation="0 0 0" animation="property: rotation; to: 0 360  0; loop: true; dur: 1000">
    <a-sphere position="1 2.5 6" color="mediumseagreen"></a-sphere>
`
* Using this code it made a sphere go clockwise and  I gave it a color of green
    * Another thing I made was another sphere but I made  it go faster than the green sphere
* The code I used for the second sphere
`
<a-entity rotation="1 2.5 6" animation="property: rotation; to:  -360 -0 0; loop: true; dur: 100">
        <a-sphere position="5 0 0" color="blue"></a-sphere>
`
##### Image of final product
![product](images/tinkering.png)

##### Code of final product
*
         <html>
         <head>
               <script src="https://aframe.io/releases/1.5.0/aframe.min.js"></script>
        </head>
               <body>
                      <a-scene>
                                 <a-box color="blue" rotation="-0 45 45" scale=" 4 4 4"  position="1 2.5  0"></a-box>
                                <a-plane rotation="-90 1.5.20" width="10" height="10" color="red"></a-plane>

                                <a-entity rotation="0 0 0" animation="property: rotation; to: 0 360  0; loop: true; dur: 1000">
                               <a-sphere position="1 2.5 6" color="mediumseagreen"></a-sphere>
                               <a-entity rotation="1 2.5 6" animation="property: rotation; to:  -360 -0 0; loop: true; dur: 100">
        <a-sphere position="5 0 0" color="blue"></a-sphere>

          </a-scene>
         </a-scene>

      </body>
    </html>
#### Challenges
* One challenge was picking an audio because I didn't know how to insert it into my IDE but then  I found out that I had to download it and just upload it

#### Questions
* How do I use animation in my Freedom project

_____


