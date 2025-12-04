# WORKSHOP-3-Canny-Edge-Detection

# Name : MOHAMMAD SHAHL
# Reg No : 212223240044


# CODE :
```
import cv2
import matplotlib.pyplot as plt
# Read the image
img = cv2.imread('mohammed.jpg',cv2.IMREAD_GRAYSCALE)
# Apply Gaussian blur to reduce noise
blurred =cv2.GaussianBlur(img, (5,5),0)
# Detect edges using Canny
edges = cv2.Canny(blurred, 50, 150) #Adjust threshold values as needed
# Plot the original image and the detected edges
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()
```
# OUTPUT :
![WhatsApp Image 2025-12-04 at 11 49 43_1aa71a2c](https://github.com/user-attachments/assets/9f3aaf78-0d90-49c0-ac56-22ac6b403335)


