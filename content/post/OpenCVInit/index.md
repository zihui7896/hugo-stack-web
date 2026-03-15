+++
date = '2025-03-22T16:10:14+08:00'
draft = false
title = 'OpenCVInit'
categories = ["OpenCV"]
description = ""
image = ""
+++

```python
# 导入 OpenCV 库，并使用别名 cv 代替 cv2
import cv2 as cv

img = cv.imread("105758.png")

# 如果图像路径错误或文件不存在，cv.imread() 会返回 None
if img is None:
    print("Error: Could not load image.")
    exit()

# "Display window" 是显示窗口的名称，可以自定义
cv.imshow("Display window", img)

# 等待按键输入
# 参数 0 表示无限等待，直到用户按下任意键
# 返回值 k 是用户按下的键的 ASCII 码值
k = cv.waitKey(0)

# 检查用户是否按下 Esc 键（ASCII 码为 27）
if k == 27:
    # 关闭所有 OpenCV 窗口
    cv.destroyAllWindows()
```

## 学习OpenCV中文版

{{< embed-pdf url="./学习OpenCV中文版.pdf" >}}



## opencv4.1中文官方文档v1.1

{{< embed-pdf url="./opencv4-1中文官方文档v1-1版.pdf" >}}
