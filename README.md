# homework4

## Take a sequence of moving-forward images in NTHU campus.
![](https://i.imgur.com/GKYU4s2.png)
---
## Show feature extraction and matching results between two images
### Feature Extraction method : ORB(Oriented FAST and Rotated BRIEF)
* Theory： ORB 基本上是 FAST 與 ORiented BRIEF 的混合，並且增加一些修改來加強表現。先利用 FAST 來尋找 keypoint，接著利用 Harris corner 來取出前 N 個最好的 keypoint。 對每個 keypoint 附近區域的像素計算 weighted centroid(把這像素灰階值當作weight)，從 keypoint 到 centroid 的方向即為該 keypoint 的 orientation。

* the moments of a patch are defined as
![](https://i.imgur.com/udSX6MD.png)
* the “center of mass(centroid)” of the patch as:
![](https://i.imgur.com/9tivBzU.png)
* The orientation of the patch is then given by
![](https://i.imgur.com/SUbefCZ.png)

### matching results between two images
![](https://i.imgur.com/MSLj8xE.png)
---
## Perform image alignment and generate infinite zooming effect
![orb zooming](https://drive.google.com/file/d/1uPSiDFjltw8JP5owMxACCPlfbZHSYUJP/view?usp=sharing)
## Implement different feature extrators

- xfeature2d SIFT

![](https://i.imgur.com/4Dvda8I.png)
- SURF

![](https://i.imgur.com/mKIuI3l.png)
## Exploit creativity to add some image processing to enhance effect.





