# Console-3D-Engine #
Program was created following the educational series "3D Console Game Engine" published by One Lonely Coder whose work can be found at:

YouTube: https://www.youtube.com/javidx9

Github: https://github.com/OneLoneCoder/

## Description ##
This series teaches the foundations of 3D graphic rendering using vector coordinates organized into matrices of triangles. User input is handled to simulate user movement, rudimentry colors and sharing are possible, and clipping occurs for both parts of the object that should be hidden by its other portions as well as portions of the object that go out of the user field of view.

### Procedure ###
1) Upon creation of matrices , the surface of each triangle is normalized against the 3D axis.
2) Because the player POV faces from the axis origin toward positive values, only surface with a negative normal are displayed.
3) Additionally any surfaces outside of the display width or height are clipped.
  * This entailes calculating new vertex points and creating multiple new triangles from a larger clipped triangle.
4) The program loops and upon receiving user input for movement will translate each vertex as needed, recreating the picture and looping through the process again.
