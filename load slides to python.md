# Intro to load image slides into python

## Load necessary libraries
``` 
%%capture
!apt-get install poppler-utils
!pip install pdf2image
from pdf2image import convert_from_path
import requests
import matplotlib.pyplot as plt
import numpy as np
from skimage.io import imread
from skimage.transform import resize
```
## Read Image from URL
```
url = 'https://raw.githubusercontent.com/williamedwardhahn/MathData24/main/boat.png'
im = imread(url)
plt.imshow(im);
```

#### Line 1: A string variable is being used to store the web address of an image.
#### Line 2: This line is used to read the image from the URL. This function turns the image into a numpy array that allows for the image to be resized or filtered.
#### Line 3: This line is used to display the image.

## Image Shape
```
im.shape
```

#### This line gives the dimensions of the object given the im variable. It outputs 3 vaulues. Height, Width, and Channels.
#### Height and Width are measured  in pixels and the channels are typically 3 for an RGB image—Red, Green, Blue—or 4 for RGBA, which includes transparency).


## Show Image
```
plt.imshow(im[0:,0:,:])
```

#### plt.imshow is a function from matplotlib that shows the image.
#### im[0:, 0:, :] slices the array to extract a certain portion of the image.

##
