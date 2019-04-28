# homework4

## Take a sequence of moving-forward images in NTHU campus.
> Draw tree
![](https://i.imgur.com/UX1BGAS.jpg)
* 可以把樹畫在天空，不像草可以排除天空的可能
> Draw grass in the sky
![](https://i.imgur.com/zUgg0dh.png)
* 不能把草畫在天空，但被畫的範圍有點綠綠的
> Draw grass
![](https://i.imgur.com/6Tj57A7.png)
> Draw brick
![](https://i.imgur.com/7cgeqAj.png)
> Remove dome
![](https://i.imgur.com/04Hozyq.png)
> Remove door
![](https://i.imgur.com/6qZoC9Y.png)
＊ 主觀來看，除了generate tree的部分有些情況會有不合理的情況產生，其他generate跟remove的效果都不錯
---
## Show feature extraction and matching results between two images
#### bed room：
![](https://i.imgur.com/SHsjrer.png)
#### Observation：
* 客廳能圈選出圖中較小較細節的物件，臥室圈選的以大物件為主，雖然是layer7但感覺效果不是最好的
---
## Perform image alignment and generate infinite zooming effect
這裡就inpainting的部分，與[Globally and Locally Consistent Image Completion](http://iizuka.cs.tsukuba.ac.jp/projects/completion/en/)(以下簡稱siggraph2017_inpainting)比較。

## exploit creativity to add some image processing to enhance effect. You can use photoshop to do some effects, such as bluring or coloring.
![](http://iizuka.cs.tsukuba.ac.jp/projects/completion/images/model_v2.png)
如上圖所示，siggraph2017_inpainting這個方法使用了三個networks，其中completion network是用來產生完整的圖片的，global和local discriminator則是幫助訓練。global discriminator能看到整張圖片，幫助達成整個圖片的連貫，local discriminator則只會看到一部份的input圖片，讓局部區域能夠一致。在訓練過程中，除了來自兩個discriminators的GAN loss以外，還加上了和原圖比較的MSE loss，讓model更加穩定。最後，對輸出的圖片有使用簡單的後處理，調整補上部分的顏色符合其四周的顏色。




