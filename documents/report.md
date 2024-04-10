# Process 
The first thing we did was withdrawing the elements from the poster and converted them into different svgs we would use to create the page. We then started writing the html with the text that gets displayed, and pasted the images into the code.

After this we started structuring the page so all the elements appear in their correct place. We used primarily positioning absolute to allign the elements to where they should be.

After that we started animating the elements, some with css animations (moving them with keyframes where we change the top attribute, transform: scale() and rotate).
We also animated the some of the svgs inside the file with SMIL, like the car and the green clouds. Making some of the paths move with transform animation.

After all the elements was animated, all that remained was some final polish to get everything positioned correctly. making sure all the elements scale correctly keeping the posters aspect ratio etc.
# recreating the waves in the background:
First we tried to draw the background "waves" in css, but realised after som time that they would be a nightmare to edit after the fact if we needed more space for elements in the poster. We then decided to use svg images instead, as it would be much easier to manage and resize if needed. 
We ended up using relative positioning on the fist wave and absolute on the other to align them correctly. We used the "vw" value in order to keep the proportions scaled for the document view window

# Animated elements
- Moon: Here we used keyframes where the positioning is moved during the animation. We wanted an effect the it appears that the mmon is floating in the air. and we think it turned out alright.
- Stars: Here we used css transform size in order to scale up and down the size of the svg images to create a pulsating animation making the stars "blink".
- Car: Here we changed the code internally of the svg making a group with the paths for ouline, fill and window of the car transform up and down a tiny amount. We did this to make it look like the engine of the car is on, and that the car is driving towards the moon.
- Humans: Here we used to forms of css animation. One where we rotate them a couple of degrees so it looks like they are walking/dancing on top of the globe. Another that translate the Y-axis so they move up and down a small amount.
- Globe: Here we did a simple rotate animation that turns the earth around 360degrees a period of time so earth is rotating. further giving into the illusion that the people on top are walking along the surface.

# css drawing:
On the first attempt we tried draw the background waves in css, but it ended up to be difficult to scale properly. insted we chose to draw the ntnu-logo in the footer with css. the logo has the class "ntnu-logo" and uses psuedoelements ::before and ::after in order to draw the squere and circle for the logo.


