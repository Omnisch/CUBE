# CUBE
A Simulator of a Rubik's Cube (without auto-solving ability) under OpenGL, MFC.

# Instruction
Key Bindings:

- Enter    Reset

- R&emsp;Right clockwise 90 degrees
- U&emsp;Up clockwise 90 degrees
- F&emsp;Front clockwise 90 degrees
- L&emsp;Left clockwise 90 degrees
- D&emsp;Down clockwise 90 degrees
- B&emsp;Back clockwise 90 degrees
- X&emsp;Rotate 90 degrees around the X-axis
- Y&emsp;Rotate 90 degrees around the Y-axis
- Z&emsp;Rotate 90 degrees around the Z-axis

- Shift + R&emsp;Right counterclockwise 90 degrees
	- etc.

- Arrows&emsp;Translate the Cube

- A&emsp;Auto-play from the beginning (after opening a formula file)

- E&emsp;Stop auto-play (after opening a formula file)

---

Mouse:

- Left click on centers&emsp;Face counterclockwise 90 degrees
- Right click on centers&emsp;Face clockwise 90 degrees
- Drag the left button&emsp;Rotate the view

---

Side Buttons:

- OpenGL
	- Antialiasing
	- Gouraud
	- Lighting&emsp;Light on/off & Switch style

	- Vertex&emsp;Vertexes only
	- Wireframes&emsp;Wireframes only
	- Face&emsp;Faces only

- Magic Cube
	- Using Textures&emsp;Use bitmaps in \res as the pattern on the Cube (customizable, but must keep the same filename)

	- Centers&emsp;Draw Centers
	- Edges&emsp;Draw Edges
	- Vertexes&emsp;Draw Vertexes

	- Rotation Limit&emsp;Limit view to F(Front) +-90 degrees

- Scaling
	- Link&emsp;Lock the scale on 1:1:1

	- X&emsp;X-scaling
	- Y&emsp;Y-scaling
	- Z&emsp;Z-scaling

- Light
	- Rotation
	- Depression
	- Distance

	- SpotLight&emsp;Switch between point light and spotlight

---

About Auto-play：

Click the "open" button,<br/>
Open a formula text file, and press A to auto-play.<br/>
Manual operations are not allowed when auto-playing; press E to quit auto-play.<br/>


The formats can be found in \res\sample_formula.txt.<br/>
The apostrophe needs to be half-width, split steps by spaces.<br/>
Auto-play will stop when encountering the first unrecognizable character.<br/>


All steps that are recognizable:<br/>
R R' R2 U U' U2 F F' F2<br/>
L L' L2 D D' D2 B B' B2<br/>
x x' x2 y y' y2 z z' z2<br/>


M(Middle) and lowercase letters(double layer) are not supported for now, please convert manually.<br/>
Counterclockwise 180 degrees is not supported for now, please convert to clockwise 180 degrees manually.<br/>
