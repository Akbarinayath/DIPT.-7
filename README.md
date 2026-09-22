#  Lane Detection

##  Aim

To implement a basic lane detection pipeline using OpenCV by completing missing code segments at specified locations.

---

## Learning Objective

* Understand each stage of image processing
* Learn how to build a complete computer vision pipeline
* Practice writing code in guided sections

**Important Instruction:**
👉 Write code **ONLY in places marked as `# Your Code Here`**
👉 Do NOT modify any other part of the code

---

##  Software Used

* Anaconda – Python 3.7
* Jupyter Notebook / VS Code
* OpenCV (cv2)
* NumPy
* Matplotlib

---

##  Algorithm & Explanation

---

###  Step 1: Import Libraries

```python
import cv2
import numpy as np
import matplotlib.pyplot as plt
```

---

###  Step 2: Read the Image

```python
# Read the image using OpenCV

image = cv2.imread('myimage.png')  

```

---

###  Step 3: Convert to Grayscale

```python
# Convert to grayscale.

gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)

```

---

###  Step 4: Display Images

```python
plt.figure(figsize=(10,5))

### INPUT IMAGE 
plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))  # Convert image to RGB for displaying
plt.title("Input Image")
plt.axis('off')

### GRAYSCALE IMAGE

plt.imshow(gray_image, cmap='gray')
plt.title("Grayscale Image")
plt.axis('off')

```

---

###  Step 5: Thresholding

```python
# Apply thresholding

threshold = 

edges = cv2.Canny(gray_image, 50, 150)

```

---

###  Step 6: Region of Interest (ROI)

```python
# ROI masking already provided
# (Do not modify)
```

---

### Step 7: Edge Detection (Canny)

```python
# Perform Edge Detection

plt.imshow(edges, cmap='gray')
plt.title("Canny Edge Detector")
plt.axis('off')

```

---

---

###  Step 8: Hough Transform

```python
# Detect lines using Hough Transform

for line in lines:
    x1, y1, x2, y2 = line  
    cv2.line(image, (x1, y1), (x2, y2), (0, 255, 0), 2)  
```

---

### Step 9: Lane Detection Logic

```python
# Already implemented
# (Do not modify)
```

---

##  Expected Output

* Original image
* <img width="417" height="492" alt="image" src="https://github.com/user-attachments/assets/4085fc92-1813-4c51-8853-789bce034ee1" />


* Grayscale image
<img width="527" height="508" alt="image" src="https://github.com/user-attachments/assets/2be0c485-fd18-41a4-93a2-f197734d7f3d" />


* Edge detected image
<img width="430" height="506" alt="image" src="https://github.com/user-attachments/assets/6ea88ab5-aa8b-464c-9867-7bd3cceba8c1" />



* Final lane detection output
<img width="470" height="498" alt="image" src="https://github.com/user-attachments/assets/174cb514-7a53-462c-91c3-b896614cba3f" />



---

##  Instructions

* Fill ONLY in `# Your Code Here` sections
* Do NOT change existing code
* Run step-by-step
* Verify outputs

---

## Result

Thus, the lane detection pipeline is successfully implemented by completing the missing code sections. The system detects and highlights lane lines effectively.

---

##  Developed By

* **Name:** AKBAR I
* **Register No:** 212224230014
