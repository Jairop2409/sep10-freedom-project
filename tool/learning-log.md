# Tool Learning Log

Tool: **Aframe**

---

3/3/24:
* watched a video about position using Aframe _*[Youtube video](https://www.youtube.com/watch?v%253DliOLtcPmMa0)_*
* read the documentation of positioning on  the Aframe [page](https://aframe.io/docs/1.5.0/components/position.html)
 ##### Things I changed  using the video
- I used aspect ratio to change the width, height, and depth of a shape, I made the `height="0.1"`, `Width="2"` `position=" 1, 0.75,-2`
 ![practice](<Aspectratio .png>)
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
![What I made](<Product.png>)

### Challenges
* The challenge I faced when trying to make new shapes using positions, width, and height was making sure it was the way I wanted and making sure the shapes/Entity had the right position( on top of the cylinder/s) I found making everything the way I wanted difficult but using the video tutorial and the Aframe webpage I was able to found out what was x,y and z in the
`a-entity position="x y z"></a-entity>
` code

### Questions
Is it possible to make an entity inside an entity code?> for example `a-circle` inside the code for `a-clyinder`?

### Next steps
* Try other components and their meaning and how I can use them on my fp(freedom) project

X/X/XX:

*
*
<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
