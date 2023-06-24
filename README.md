
![header](https://capsule-render.vercel.app/api?type=Waving&color=auto&animation=fadeIn&height=160&section=header&text=Fabric%20Defects%20Detector&fontSize=60)


## Introduction
The most common problem with manual inspection would be human errors while detecting the defects and calculating the correct lengths to cut. This will lead to higher wastage of fabric when cutting. This is a simple solution to detect defects in plain-colored fabrics using the OpenCV library. This uses contours to identify the weaknesses in plain-coloured materials and calculates the total wastage of fabric due to the defects.


## Approach
1. Get the video stream of the fabric moving through the machine.
2. Break the video into frames.
3. Convert the frames to grayscale.
4. Apply Gaussian blur to reduce the noise.
5. Convert the resulting image to a binary image.
6. Apply morphology close operation to close the gaps between pixels.
7. Calculate contours.
8. Calculate the bounding rectangle for each contour.
9. Calculate the wastage by using the calculated values and the minimum piece length.
10. Show the results.
    
### Prerequisites
Install 
[Python3](https://www.python.org/downloads/)
[opencv V3.0+](https://pypi.org/project/opencv-python/)
[NumPy V1.0+](https://pypi.org/project/numpy/)

### Installation

### Usage
First, clone this project
```sh
git clone https://github.com/ravdsn/morse-code-translator.git
cd morse-code-translator 
```
Then, run morseCodeTranslator.py 
```sh
python3 morseCodeTranslator.py 
```

## Screenshots

![Identified defects](/screenshots/1.jpg)
![Wastage](/screenshots/2.jpg)


![header](https://capsule-render.vercel.app/api?type=rounded&color=gradient&text=%20Warning⚠️%20-nl-%1GGives%20some%20error%20with%20opencv%20old%20versions%1&animation=blinking&height=100&fontSize=30)
##

![footer](https://capsule-render.vercel.app/api?type=Waving&color=auto&animation=fadeIn&height=160&section=footer)




