# Running the software
Running this testbed requires downloading some additional software:

 - [Java 3D 1.5.1](http://www.oracle.com/technetwork/java/javasebusiness/downloads/java-archive-downloads-java-client-419417.html#java3d-1.5.1-oth-JPR) 
	 - `j3dcore.jar`
	 - `j3dutils.jar`
	 - `vecmath.jar`
	 - native library (`.so` or `.dll` file)
 - [QuickHull3D](https://www.cs.ubc.ca/~lloyd/java/lib/quickhull3d.jar)
	- `quickhull3d.jar`

To run the program, make sure it's parent directory includes every `.jar` you downloaded. Additionally, you should link the native library's parent directory using the `java.library.path` option. For example, assuming all files reside in the same directory, you should use:

	`java -Djava.library.path=. -jar peno.jar`

# Using the software
Running the testbed will spawn a file-selection screen. Select a world description file (cancel the selection will load an empty world). To move around in the world click on the camvas in the testbed and use the ¨WASD¨ keys and the arrows to rotate in the world. Add your autopilot by connecting to `localhost:8000` using the wire protocol. Click the buttons in the GUI to start or pause the simulation.

Loading a new while there is a drone in the simulator will keep the drone in the previous world. Reconnect the autopilot in this case.

# Remarks
As this is the first version of our testbed it could contain some mistakes. Please report all your issues via the Issues tab of this website.
