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

#### 
dddd
