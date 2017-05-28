### IMPORTANT

This project was my very first project in C++ (I primarily used Java before), therefore there will be many memory leaks, weird programming styles and also changes in my style of coding. 

<img src="https://raw.githubusercontent.com/add-ryan/vxl/master/vxl%20logo.png" height=200/>

### What is VXL?
* VXL is a voxel-octree rendering engine running on OpenCL (OpenGL is used for displaying only)
* (At the moment) it is using a tree based per-pixel search algorithm for rendering voxel models
* The project is work in progress and not nearly near a finished state and can be seen as an experiment
* At the moment it is not open source, however I plan on publishing the source code at some time
* The latest version is VXL Alpha 1.3

### Features
* The program can convert triangulated OBJ-models into VXL-models with a uniform colour
* Certain variables like resolution, OpenCL-device and so on can be changed in properties files contained within ./props
* VXL can render 3D voxel models of any size at any resoution as far as they don't exceed the computers memory
* You view the models from any perspective using WASD for the camera movenent and the arrow keys for the rotation
* The project is written in C/C++, it can and will in the future therefore be ported to Linux and OSX

### Future Plans
* VXL is supposed to become a game engine at some point, however it is still far from that
* The idea is that using search algorithms for rendering, "unlimited" detail can be achieved

### Requirements
* Graphics card that supports OpenGL, OpenCL and recursion
* Microsoft Visual C++ 2015 (get it [here](https://www.microsoft.com/en-us/download/details.aspx?id=48145 "Microsoft Visual C++ 2015"))
* The required memory (also on the GPU) depends on the size of the model you are rendering

### How to run VXL</h1>
* Download the file named "vxl.<version>.zip" desired version [here](https://github.com/add-ryan/vxl/releases "Releases")
* Extract the folder and modyfy ./props/graphics.properties and ./props/OpenCL.properties to fit your setup
* Run either "run.bat" or "Voxel.exe"

### Preview (VXL Alpha 1.3)
* The shown model is an octree with 10 subdivisions (model resolution of 1024x1024x1024, screen resolution of 500x500)
* Used GPU: NVIDIA GTX 750Ti
* The Polygonal structure in this preview is due to the original model not being very large
* The .vxl file is ~400MB in size. For reference: each cube contains 3 normal values (32-bit floats) and one colour (32-bit unsigned int), file size for this model using a simple 1024x1024x1024-matrix would be 16GB

![Preview](https://cloud.githubusercontent.com/assets/23387365/21947686/b307a83a-d9e6-11e6-851d-01f015b8e8b1.PNG)
