# DIPT
## steps:
### Read the image ('Apollo-11-launch.jpg')
### Print the image width and height.
### Display the image using matplotlib
### Display the image using matplotlib
## program:
```
import cv2
import matplotlib.pyplot as plt
image = cv2.imread("jjj.jpeg")
fig, ax = plt.subplots()
ax.imshow(image)
ax.set_xticks(range(0, image.shape[1], 100))
ax.set_yticks(range(0, image.shape[0], 100))
plt.show()
image = cv2.imread("jjj.jpeg")
x, y = 500, 50
width = 200
height = 600
cv2.rectangle(image, (x, y), (x + width, y + height), (0, 0, 255), 3)
fig, ax = plt.subplots()
ax.imshow(image)
ax.set_xticks(range(0, image.shape[1], 100))
ax.set_yticks(range(0, image.shape[0], 100))
plt.show()
```
## program-2:
```
import cv2
import matplotlib.pyplot as plt

image = cv2.imread('lake.jpeg', cv2.IMREAD_COLOR)

print("Color image shape:", image.shape)

gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)

print("Grayscale image shape:", gray_image.shape)

plt.figure(figsize=[10, 10])
plt.imshow(gray_image, cmap='gray')  
plt.show()
```
## program-3
```
import cv2
import matplotlib.pyplot as plt

# Step 1: Read the saved image ('Emerald_Lakes_New_Zealand.jpg') as a color image.
image = cv2.imread('Emerald_Lakes_New_Zealand.jpg', cv2.IMREAD_COLOR)

# Step 2: Print the image shape.
print("Color image shape:", image.shape)

# Step 3: Convert the image to grayscale using cv2.cvtColor().
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)

# Step 4: Print the grayscale image shape.
print("Grayscale image shape:", gray_image.shape)

# Step 5: Display the grayscale image using matplotlib imshow.
plt.figure(figsize=[10, 10])
plt.imshow(gray_image, cmap='gray')  # Displaying in grayscale
plt.show()
```
## output:
![image](https://github.com/user-attachments/assets/334cded5-60aa-4c6f-852d-e154cc7f57a7)
![image](https://github.com/user-attachments/assets/a8789d3f-a0b4-4c95-a36e-27d60f2942fd)
![image](https://github.com/user-attachments/assets/06b4f985-c648-48d1-9837-5159487db5ae)




