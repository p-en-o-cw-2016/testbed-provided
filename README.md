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
Running the testbed will spawn a file-selection screen. Select a world description file, and use the WASD keys to move around in the newly generated world. Add your autopilot by connecting to `localhost:8000` using the wire protocol. Click the buttons in the GUI to start or pause the simulation.