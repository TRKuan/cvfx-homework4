# homework4

## Take a sequence of moving-forward images in NTHU campus.
![](https://i.imgur.com/GKYU4s2.png)
---
## Show feature extraction and matching results between two images
### Feature Extraction method1 : ORB(Oriented FAST and Rotated BRIEF)
* Theory： ORB 基本上是 FAST 與 ORiented BRIEF 的混合，並且增加一些修改來加強表現。先利用 FAST 來尋找 keypoint，接著利用 Harris corner 來取出前 N 個最好的 keypoint。 對每個 keypoint 附近區域的像素計算 weighted centroid(把這像素灰階值當作weight)，從 keypoint 到 centroid 的方向即為該 keypoint 的 orientation。


---
## Perform image alignment and generate infinite zooming effect


## exploit creativity to add some image processing to enhance effect. You can use photoshop to do some effects, such as bluring or coloring.





