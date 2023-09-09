# CUBE
A Simulator of a Rubik's Cube (without auto-solving ability) under OpenGL, MFC.

# Instruction
Key Bindings:

Enter    Reset

R    Right clockwise 90 degrees
U    Up clockwise 90 degrees
F    Front clockwise 90 degrees
L    Left clockwise 90 degrees
D    Down clockwise 90 degrees
B    Back clockwise 90 degrees
X    Rotate 90 degrees around the X-axis
Y    Rotate 90 degrees around the Y-axis
Z    Rotate 90 degrees around the Z-axis

Shift + R    Right counterclockwise 90 degrees
etc.

Arrows    Translate the Cube

A    Auto-play from the beginning (after opening a formula file)

E    Stop auto-play (after opening a formula file)


================

Mouse:

Left click on centers    Face counterclockwise 90 degrees
Right click on centers    Face clockwise 90 degrees
Drag the left button    Rotate the view


================

Side Buttons:

OpenGL
	Antialiasing
	Gouraud
	Lighting    Light on/off & Switch style

	Vertex    Vertexes only
	Wireframes    Wireframes only
	Face    Faces only

Magic Cube
	Using Textures    Use bitmaps in \res as the pattern on the Cube (customizable, but must keep the same filename)

	Centers		Draw Centers
	Edges		Draw Edges
	Vertexes		Draw Vertexes

	Rotation Limit	Limit view to F(Front) +-90 degrees

Scaling
	Link    Lock the scale on 1:1:1
	X    X-scaling
	Y    Y-scaling
	Z    Z-scaling

Light
	Rotation
	Depression
	Distance

	SpotLight    Switch between point light and spotlight


================

About Auto-play：

Click the "open" button,
Open a formula text file, and press A to auto-play.
Manual operations are not allowed when auto-playing; press E to quit auto-play.

The formats can be found in \res\sample_formula.txt.
The apostrophe needs to be half-width, split steps by spaces.
Auto-play will stop when encountering the first unrecognizable character.

All steps that are recognizable:
R R' R2 U U' U2 F F' F2
L L' L2 D D' D2 B B' B2
x x' x2 y y' y2 z z' z2

M(Middle) and lowercase letters(double layer) are not supported for now, please convert manually.
Counterclockwise 180 degrees is not supported for now, please convert to clockwise 180 degrees manually.
