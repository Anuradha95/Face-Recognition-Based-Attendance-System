# Face-Recognition-Based-Attendance-System
INTRODUCTION

Attendance is carried out to have proper count of people or students in a particular classroom, meeting or any practice area. Our aim is to digitize the process of taking attendance and make it simple and 
accurate by using image processing technique.

PROCESS

  First, lock at the picture and find the face in that image

  Second, focus on the face and check whether the face is in a bad lighting condition or turned to wired direction.

  In the third step measure the face and encode the data.
  
  Finally, determine the person's name by comparing the taken encoded data with known encoded data sets.

LIBRARY Face-Recognition

1. Finding a face
The first step is face detection. The method used in this process is called Histogram of Oriented 
Gradients (HOG). First the image is converted into a black and white image. Then check every 
single pixel in the image with its four neighbors and find out how darker the current pixel with 
compared to four neighbors. Then every pixel is replaced by an arrow flow from light to dark. 
These arrows are called “Gradient”. After that, using those arrows make the HOG version of the 
image

2. Detect the same face in different angle
In this case we use a new technique to identify faces. That algorithm is called face landmark 
estimation. This algorithm train finds the 68 specific points on any face. Then do the affine 
transformation (basic image transformations like rotation and scale that preserve parallel lines) to 
center the eyes mouth and nose as much as possible

3. Encoding
Uses a trained network to find embedding (128 measurements of each face) of a face.

4. Identifying the person
Find the person in our database of known people who has the closest measurements with our test 
image.

Result
[Attendance.csv](https://github.com/Anuradha95/Face-Recognition-Based-Attendance-System/files/8825127/Attendance.csv)

