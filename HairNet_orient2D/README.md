# Orientation Map

## HairNet_orient2D
https://github.com/papagina/HairNet_orient2D

This repo contains the code for generating the orientation images in the paper HairNet: Single-View Hair Reconstruction using Convolutional Neural Networks.

## Instruction

```Workspace``` <br>
Docker Container 

### Compile
Compile the code in Hair_Orient2D.

Please check the CMakeLists for dependencies.
* OPENGL, GLEW, GLFW3 and OpenMesh are only used for rendering a white body silhouette. If you don't need it, you can simply remove them and compile with the optional main_nobodyrender.cpp.

### Run
Compute 2D orienation maps from portrait images in given folder.

**Use command:** <br>
Hair_Orient2D/Orient2D test_imgs/

**Note:** <br>
 all the directory arguments need to have "/" at the end of the string.<br>

 Put the test imgs in "test_imgs/img/", the test images should be square, e.g. 800*800

 Put the segment images in "test_imgs/seg/hair/", with the same name as in img folder, XXX.png. hair is white, background is black


### Additional
hair-segmented images can be made using the [segmentation repo](https://github.com/givenone/hair-segment)
