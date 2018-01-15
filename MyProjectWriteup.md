# **Finding Lane Lines on the Road** 

## Lesson 2 Project: Lane Finding for Images and Videos

### You can use the [Dillinger](https://dillinger.io) website to update markdown files.  Document formats other than Markdown would also be useful as well.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
1. Continue learning some common industry software development languages and environments (e.g. Jupyter notebooks, Anaconda, Markdown files, Git, etc.)
2. Functionalize some of the code blocks in the prior lessons
3. Introduce some common Python libraries and their class functions
    a. **Lesson Libraries**: `matplotlib`, `numpy`, OpenCV `cv2`
    b. **New Libraries from Project**: `moviepy`, `IPython` 
    c. **Useful General Libraries**: File/System `os`, Math `math` 
4. Reflect on your work in a written report

[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Lesson 2 Project Outline & Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

In this lesson's project we needed to fork the project on GitHub, update our forked project's jupyter notebook code cells, create our writeup, and push our code changes back to our GitHub forked repository.

1. Lesson 2 Project Setup:
    * Follow instructions for initial setup and testing of Anaconda
    * Create a GitHub account if you don't already have one
    * Fork the Lesson 2 Project (will show up in your GitHub page)
    * Clone the forked repo to your local computer
    * Follow instructions for opening the jupyter notebook inside the cloned repo.
2. Lesson 2 Project Default Jupyter Code Blocks (Building Block Cells):
    * Code Cell 1: Import Python libraries needed for other cell block (No Change)
    * Code Cell 2: Load a project image and display in jupyter notebook (No Change)
    * Code Cell 3: Define/Create the local project functions learned from prior lessons (Major Coding Section):
        * grayscale(): Convert color image to grayscale image
        * canny(): Apply the Canny transform to an image based on input values
        * gaussian_blur(): Apply Gaussian blurring (Gaussian noise kernel) to an input image based on input values
        * region_of_interest(): Apply an image blanking mask to an input image based on input parameters
        * draw_lines(): Function that draws lines "inplace" on an image based on the input parameters.
        * hough_lines(): Draws "Hough lines" on an image based on the input parameters
        * weighted_img(): 
3. Lesson 2 Project Default Jupyter Code Blocks (Image & Video Processing Cells):
    i. Image Processing Cells
    * Code Cell 4: Write the code to load the images from the "Test Images" directory in the cloned project.  For each image, load image, run lane finding algorithm, and save to a file.

    ii.  Video Processing Cells
    * Code Cell 5: Import the video processing libraries (Nothing to do but run this cell)
    * Code Cell 6: Define the video processing library code
    * Code Cell 7: Write the code to load the videos from the "Test Videos" directory in the cloned project.  For each video, load video, run lane finding algorithm, and save to a file.
    * Code Cell 8: Preview the video in the jupyter notebook (nothing to do but run this cell)
    * Code Cells 9-12: Repeat video processing code cells 7 & 8 


If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline


Definitely need to refine the lane finding algorithm to look at the slop of the lines more for excluding things like the cars (which are near zero slope). Making the lines more solid would have been nice but spent more time learning about the Python language than getting to play with the math (I think Python was created when C and Matlab had a kid, but was then adopted by another programming language somewhere along the way).


### 3. Suggest possible improvements to your pipeline

Going thru the code to refine the lane finding in more detail so that extraneous items outside the closest lanes are needed.  Didn't have time play with everything as much as I would like, and don't want to get behind on the course.

