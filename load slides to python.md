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

####Line 1: A string variable is being used to store the web address of an image.
####Line 2: This line is used to read the image from the URL. This function turns the image into a numpy array that allows for the image to be resized or filtered.
####Line 3: This line is used to display the image.
