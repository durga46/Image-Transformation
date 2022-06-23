## EX.NO : 05
## Date : 27.04.2022
# <p align="center"> Image-Transformation</p>
## Aim
To perform image transformation such as Translation, Scaling, Shearing, Reflection, Rotation and Cropping using OpenCV and Python.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import the necessary libraries and read the original image and save it a image variable.
<br>

### Step2:
Translate the image using Translation_matrix=np.float32([[1,0,120],[0,1,120],[0,0,1]]) Translated_image=cv2.warpPerspective(org_img,Translation_matrix,(col,row))
<br>

### Step3:
Scale the image using Scaling_Matrix=np.float32([[1.2,0,0],[0,1.2,0],[0,0,1]]) Scaled_image=cv2.warpPerspective(org_img,Scaling_Matrix,(col,row))
<br>

### Step4:
Shear the image using Shearing_matrix=np.float32([[1,0.2,0],[0.2,1,0],[0,0,1]]) Sheared_image=cv2.warpPerspective(org_img,Shearing_matrix,(col2,int(row1.5)))
<br>

### Step5:
Reflection of image can be achieved through the code Reflection_matrix_row=np.float32([[1,0,0],[0,-1,row],[0,0,1]]) Reflected_image_row=cv2.warpPerspective(org_img,Reflection_matrix_row,(col,int(row)))
<br>

### Step6:
Rotate the image using Rotation_angle=np.radians(10) Rotation_matrix=np.float32([[np.cos(Rotation_angle),-np.sin(Rotation_angle),0], [np.sin(Rotation_angle),np.cos(Rotation_angle),0], [0,0,1]]) Rotated_image=cv2.warpPerspective(org_img,Rotation_matrix,(col,(row)))
<br>

### Step7:
Crop the image using cropped_image=org_img[10:350,320:560]
<br>

### Step8:
Display all the Transformed images.
<br>

## Program:
```python
Developed By:DurgaDevi P
Register Number:212220230015
i)Image Translation
Translation_matrix=np.float32([[1,0,120],[0,1,120],[0,0,1]])
Translated_image=cv2.warpPerspective(original_img,Translation_matrix,(col,row))
plt.axis("off")
plt.imshow(Translated_image)

ii) Image Scaling
Scaling_Matrix=np.float32([[1.2,0,0],[0,1.2,0],[0,0,1]])
Scaled_image=cv2.warpPerspective(original_img,Scaling_Matrix,(col,row))
plt.axis("off")
plt.imshow(Scaled_image)

iii)Image shearing
Shearing_matrix=np.float32([[1,0.2,0],[0.2,1,0],[0,0,1]])
Sheared_image=cv2.warpPerspective(original_img,Shearing_matrix,(col*2,int(row*1.5)))
plt.axis("off")
plt.imshow(Sheared_image)

iv)Image Reflection
Reflection_matrix_col=np.float32([[-1,0,col],[0,1,0],[0,0,1]])
Reflected_image_col=cv2.warpPerspective(original_img,Reflection_matrix_col,(col,int(row)))
plt.axis("off")
plt.imshow(Reflected_image_col)

Reflection_matrix_row=np.float32([[1,0,0],[0,-1,row],[0,0,1]])
Reflected_image_row=cv2.warpPerspective(original_img,Reflection_matrix_row,(col,int(row)))
plt.axis("off")
plt.imshow(Reflected_image_row)

v)Image Rotation
Rotation_angle=np.radians(10)
Rotation_matrix=np.float32([[np.cos(Rotation_angle),-np.sin(Rotation_angle),0],
                                [np.sin(Rotation_angle),np.cos(Rotation_angle),0],
                                [0,0,1]])
Rotated_image=cv2.warpPerspective(original_img,Rotation_matrix,(col,(row)))
plt.axis("off")
plt.imshow(Rotated_image)

vi)Image Cropping
cropped_image=original_img[10:350,320:560]
plt.axis("off")
plt.imshow(cropped_image)
```
## Output:
### i)Image Translation
![s2](https://user-images.githubusercontent.com/75235704/165687471-dc53fb34-4b8d-49da-9901-60e3c0294a36.png)
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

### ii) Image Scaling
![s3](https://user-images.githubusercontent.com/75235704/165687648-35862b38-f05d-4d72-9425-36fac80b9152.png)
<br>

### iii)Image shearing
![s4](https://user-images.githubusercontent.com/75235704/165688178-ae23b83c-8730-48be-ae9f-d54b649ceb73.png)
<br>

### iv)Image Reflection
![s5](https://user-images.githubusercontent.com/75235704/165688029-e6375727-32fd-4636-95f7-17f8b8d14fdb.png)
![s6](https://user-images.githubusercontent.com/75235704/165688042-b89f1bde-62c8-4ab9-98dc-ad811b1a572d.png)
<br>
<br>
<br>
<br>



### v)Image Rotation
![s7](https://user-images.githubusercontent.com/75235704/165688115-6aa08e98-4cf9-418d-94d9-ff86a755754e.png)
<br>
<br>
<br>
<br>



### vi)Image Cropping
![s8](https://user-images.githubusercontent.com/75235704/165688066-e2380c3c-32f4-4990-bf8f-004426ad8c1c.png)
<br>
<br>
<br>
<br>




## Result: 

Thus the different image transformations such as Translation, Scaling, Shearing, Reflection, Rotation and Cropping are done using OpenCV and python programming.
