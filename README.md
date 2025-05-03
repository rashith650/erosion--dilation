# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>
Import required libraries (OpenCV, NumPy) and load the image in grayscale.


### Step2:
<br>
Define a structuring element (kernel) for morphological operations.



### Step3:
<br>
Apply erosion using cv2.erode() on the image with the defined kernel.



### Step4:
<br>
Apply erosion using cv2.erode() on the image with the defined kernel.



### Step5:
<br>
Display and compare the original, eroded, and dilated images.




 
## Program:

``` Python
mport cv2
import numpy as np
import matplotlib.pyplot as plt

image = np.zeros((500, 500, 3), dtype=np.uint8)

font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(image, 'Hello World', (100, 250), font, 1, (255, 255, 255), 2, cv2.LINE_AA)
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))  # Convert BGR to RGB for displaying
plt.title("Input Image with Text")
plt.axis('off')

kernel = np.ones((3, 3), np.uint8)

eroded_image = cv2.erode(image, kernel, iterations=1)

plt.imshow(cv2.cvtColor(eroded_image, cv2.COLOR_BGR2RGB))  # Convert BGR to RGB
plt.title("Eroded Image")
plt.axis('off')

dilated_image = cv2.dilate(image, kernel, iterations=1)

plt.imshow(cv2.cvtColor(dilated_image, cv2.COLOR_BGR2RGB))  # Convert BGR to RGB
plt.title("Dilated Image")
plt.axis('off')
```
## Output:

### Display the input Image
![image](https://github.com/user-attachments/assets/37255113-5822-41f5-9b9f-429744ec7d7c)


### Display the Eroded Image
![image](https://github.com/user-attachments/assets/58157f0e-3986-498f-9327-1dc3c4d61be0)


### Display the Dilated Image
![image](https://github.com/user-attachments/assets/cafdacf7-3d86-4e05-83f7-8737c1040dba)


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
