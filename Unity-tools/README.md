# What's this?

Unity tools is a script that handles the famous rotation problem when you work with Blender and Unity.

In most case we store our model as fbx file then import it into Unity. But Unity is using Y-up axis while Blender is using Z-up axis. That comes the problem.

# Any quick fix?

Sure! 
* Rotate your model to -90 degrees and apply rotation manually. ``CONS``: It makes harder to change your model somewhat.
* Add an empty parent gameobject to your model in Unity scene. ``CONS``: It's horrible if you want to GetComponent() from your scripts directly since GetComponentInChildren() is way slower. Unity wrote this in their guide line, but trust me, it sucks :\ In real life, it's much handy to attach scripts on model directly other than an meaningless empty parent.

# What can this script do?

Keep your model rotation correctly both in Unity and Blender.

# More info?
Source: http://forum.unity3d.com/threads/blender-unity-rotation-fix.181870/

