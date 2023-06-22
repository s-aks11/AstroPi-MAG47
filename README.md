# AstroPi-MAG47
AstroPi Mission Space Lab 
Team: Magnet 47

*************************************************

Table of Contents

1. Project Description
2. Files required
3. Internal workings
4. Testing
5. Credits 

*************************************************

1. Project Description

This program is designed to process NDVI (Normalized Difference Vegetation Index) mapped images and convert them into 6 by 6 numerical matrices so that the index values can be compared for vegetation vitality analysis.

*************************************************

2. Files Required

Before running this code, ensure that you have the following dependencies installed:

PIL (Python Imaging Library)
NumPy

This program requires the mapped NDVI images classified in a folder labeled 'images' in the current directory. 

*************************************************

3. Internal Workings

This program utilizes multiple procedures/functions to successfully run. These are listed below (in order) as well any other information relevant to the code. 

1. Ensure all images are in the correct folder labelled 'images'. 
2. Update the folder_path variable in the code to match the folder path where your images are stored.
3.Run the script.

The code will iterate over each image in the specified folder and perform the following steps:

1. Load the image.
2. Convert the image to a NumPy array.
3. Check if the image array has three or more bands.
4. Extract the red and near-infrared bands from the image array.
5. Calculate the NDVI values using the calculate_ndvi() function.
6. Print the NDVI values as desired. 

Note: The current implementation assumes that the red band is at index 0 and the near-infrared band is at index 2 of the image array. The nir_band index can be modified if needed. 
*************************************************

4. Testing

To ensure that our program will be successful, we completed multiple tests throughout our design. Some of the scenarios executed include: 

- Performed unit testing by testing individual procedure(s).
- Ran the program end-to-end for a selected variety of images. 
- Ran the program end-to-end for all images.
 
*************************************************

5. Credits
Teacher/Mentor: Mr. Christopher McFadden
Group Members: Akshita Sharma, Jessica Anirisaihan 
School: O’Neil CVI, Oshawa, ON, Canada

*************************************************
