ImageReducer
============

To use this software:

1. Put your original images in 'originals' directory

2. Run "Reducer'
e.g. In Eclipse, right-click/Command-click on Reducer in the Package Explorer View and select "Run As Java Application"

3. Reduced versions of the images appear in output directory
Hint: In Eclipse, right-click/Command-click on the project name and select Refresh(F5) for them to show up.
You can then copy-paste them to where you need them

Typical output:
Processing originals/illiac1.jpg
Source width,height : 2560,1920
Output width,height : 640,480
Memory requirements : 1200 KB
Output file:output/4.0/illiac1.jpg, file size : 347 KB


To change the reduction factor edit Reducer.java :
The default reduces the memory requirements of the image by 1/16th:

double factor = 4; 

- the output image is a 1/4th of the width and 1/4th of the height

e.g.
double factor = 3;

This will create output images that are three times smaller
i.e. require about 1/9th of the memory.
