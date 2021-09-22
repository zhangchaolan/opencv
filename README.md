# 图像色彩转换
import cv2 as cv
import numpy as np
image1=cv.imread("C:/111/caise.png")
cv.imshow("image1",image1)
image2=cv.cvtColor(image1,cv.COLOR_BGR2RGB)
image3=cv.cvtColor(image1,cv.COLOR_BGR2GRAY)#八位灰度图
image4=cv.cvtColor(image2,cv.COLOR_BGR2YCrCb)#弥补了亮度信息，Y表示亮度
image5=cv.cvtColor(image2,cv.COLOR_BGR2HSV)#色调，饱和度，亮度三要素
cv.imshow("image2",image2)
cv.imshow("image3",image3)
cv.imshow("image4",image4)
cv.imshow("image5",image4)
cv.waitKey()
cv.destroyAllWindows
