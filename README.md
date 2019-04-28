# homework4

## Take a sequence of moving-forward images in NTHU campus.
![](https://i.imgur.com/GKYU4s2.png)
---
## Show feature extraction and matching results between two images
### Feature Extraction method1 : ORB(ORiented Brief)
* 原理簡介： ORB 基本上是方法 FAST 與 BRIEF 的結合，再加上許多的修改來增加效能，一開始先使用 FAST 來搜尋 keypoint，再將所搜尋出來的結果，用 Harris corner 來取出前 N 個最有可能是 corner 的 keypoint。 對每個 keypoint 附近區域的像素計算其 weighted centroid(以各像素的灰階值為weight)，從 keypoint 到其 weighted centroid 的方向即為該 keypoint 的 orientation。
---
## Perform image alignment and generate infinite zooming effect


## exploit creativity to add some image processing to enhance effect. You can use photoshop to do some effects, such as bluring or coloring.





