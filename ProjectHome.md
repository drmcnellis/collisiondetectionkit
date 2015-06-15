--NOTICE--

A new version of the CDK is now available! Updates have been made based on user feedback, as well as overall code optimization. Download the new CDK v1.5 and enjoy these changes:

- "overlap" property in the checkCollisions() returned array has been replaced by "overlapping".  The new overlapping property is an array of all the pixels that were overlapping in the collision, given to you in stage coordinates.  Now you can know exactly **where** your collisions are happening as well as by how much.

- You no longer need to have display objects on the stage to detect for collisions!  Use the CDK in your blitting engines and experience the added speed benefits of detecting for collisions off the stage with the CDK.  Works with objects on the stage colliding against objects off the stage.  The display list simply doesn't matter anymore!

- Transformations made on parent display objects are now accounted for.  Do whatever you want to your container sprites without fear of it messing with your collision detection.

- Code optimizations have led to ~15% in speed improvements overall.

If you're already using the CDK, I strongly encourage you to get this new version. Please note that the package name has changed, and now resides at com.coreyoneil.collision

Enjoy!  And as always, if you use the CDK in a project, feel free to let me know.  The CDK has had over 2500 downloads so far, and I love hearing about the cool things devs are using this for.  :)

--/NOTICE--




The Collision Detection Kit is a package of classes created for pixel-precise, shape-based collision detection for all display objects. It is written in Actionscript 3.0 and meant for Flash Player version 9 and higher.
The Collision Detection Kit comes with several features to control how collisions are detected, and provides data for the user of the class so they can do something about the collision:

  * Set an alpha threshold to ignore colors below the threshold.
  * Specify colors and color ranges to exclude from collision detection.
  * Receive an angle of collision for each collision. We're not talking about bounding boxes here - the angle is calculated based on the shapes of the display objects at the site of the collision. Great for when you're working with physics!
  * Receive the pixels that overlapped in a collision in stage coordinates. Combined with the returned angle, and your physics engine will have no problems traversing complicated shapes or performing off-axis rotation.
  * Takes transformations (scale, rotation, color transforms, etc.) of individual instances of your display objects into account.
  * Add items for collision detection regardless of their nesting.
  * You can have as many CollisionGroup and CollisionList instances as you want, allowing you to easily manage different interactions and behaviors.
  * Works with all display objects - MovieClips, Sprites, Bitmaps, TextFields, FLVs, and on and on!


To learn more about this package and how to use it, please reference the links for examples and documentation.

The CDK is released under the MIT license.  Copyright 2008, Corey O'Neil www.coreyoneil.com