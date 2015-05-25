---
layout: post
title: 3D Printing with MakerBot and OpenSCAD
---

###Basic 3D Printing with MakerBot Thingverse

In this section we are going to get started with some basic 3D Printing. That is, we are going to customize some premade objects from [MakerBot Thingiverse](http://www.thingiverse.com/customizable){:target="_blank"} 

If you want build and code your own 3D objects from scratch (which is awesome but a little harder), then take a look at the [Advanced 3D Printing section](###Advanced 3D Printing with OpenSCAD
).

Here are some cool objects that have been preselected for you to customize:

[iPhone 4/5/6 Case](http://www.thingiverse.com/apps/customizer/run?thing_id=813330){:target="_blank"}

[Dog Tag](http://www.thingiverse.com/apps/customizer/run?thing_id=774035){:target="_blank"}

###Advanced 3D Printing with OpenSCAD

If you are familiar with some basic Geometry, then you already know about the X and Y axis that make up a 2D plane like in the one below:

![2D Plane]({{ site.baseurl }}/images/plane.png){:.img-normalize}

When we are making 3D models, we are going to be designing them on a 3D plane. As such, there is another axis we need to concern ourselves with called the Z axis. The Z axis is third dimension we are talking about when we talk about 3D. So, when we are modeling things for the 3D printer, we must take into consideration the X, Y, and *Z* axis.

![Z Axis]({{ site.baseurl }}/images/zaxis.png){:.img-normalize}

So, with that in mind, let's get started:

Now, with OpenSCAD we are going to be programming our 3D objects. By that I mean using only text that looks similar to other programming languages like Java, we will build 3D objects. This may seem a bit frustrating and cumbersome at first. I mean, why can't we just manipulate things visually using the mouse! 

Not to worry! I can assure you that with practice you will get the hang of and realize the power of being able to manipulate 3D objects using just the text that you type.

#####[Download OpenSCAD](http://files.openscad.org/OpenSCAD-2015.03-1.dmg){:target="_blank"}

Open the OpenSCAD program you just downloaded (double click the OpenSCAD-2015.03-1.dmg file).

See below for some important buttons you will use when building your objects.

![Buttons]({{ site.baseurl }}/images/buttons.png){:.img-normalize}

Let's do a couple of simple things, like make a cube that is 10x20x30 millimeters in size.

In your editor on the right side of the OpenSCAD window type the following.

	cube(size = [10,20,30], center = true);

Then press the 'Preview' button to see what it looks like.

![preview]({{ site.baseurl }}/images/preview.png)

You should see a cube in your preview pane.

Notice the syntax of our command. We ask for a cube and specify its size.

That is, [10,20,30] where those numbers correlate to the [X,Y,Z] axis. Try fiddling with those numbers to change the size.

Also, note that millimeters are a metric measurment. You can convert millimiters to inches on various websites. But an inch is about 25 millimeters.

Let's try a sphere. Type:

	sphere(d = 40);

And press the preview button again.

In this case, we are telling the program to create a sphere of size 40 millimiters. The 40 mm in this case corresponds to the diameter of the sphere.

Finally, let's make something a little more complicated (and useful) by combining the simple things we have done so far.

Now, OpenSCAD can get really complicated, so those simple examples and then you can go down the "rabbit hole" of the OpenSCAD documentation on your own [here](http://en.wikibooks.org/wiki/Category:OpenSCAD_User_Manual).
