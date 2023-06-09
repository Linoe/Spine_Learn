# Spine 人體關節

演示如何製作關節

> IK 參考[Spine_骨架約束](Spine_骨架約束.md)

## 人體關節

![](moive/2023-03-18%2017_44_51.webp)

> 先準備好圖片網格
> <br>
> ![](img/2023-03-18%2017_24_29.png)
> ![](img/2023-03-18%2017_24_46.png)
> ![](img/2023-03-18%2017_24_56.png)

![](moive/2023-03-18%2017_39_44.webp)

1. 建立符合圖片的骨架，並綁定對應的圖片
3. 建立 IK 約束

+ 綁定骨架時，連接的骨架一起綁定，動作時不會破圖
  <br>
  ![](img/2023-03-18%2017_49_31.png)
  ![](img/2023-03-18%2017_49_52.png)

## 生動的關節

![](moive/2023-03-18%2020_29_03.webp)

設置外部 IK 骨架，另圖片第一節骨架對應伸縮

1. 建立符合圖片的骨架，並綁定對應的圖片
2. 在外部建立一組輔助用的骨架
3. 圖片第一節的骨架建立單一 IK ，外部骨架建立一組 IK，外部與內部骨架同一層級
   <br>
   ![](moive/2023-03-18%2018_32_19.webp)
   ![](img/2023-03-18%2020_25_58.png)
4. 圖片第一節的 IK 目標端與外部第二節的骨架綁定變換約束
   <br>
   當綁定完無法動作時，需要調整約束順序
   <br>
   ![](moive/2023-03-18%2019_51_57.webp)
5. 圖片第二節的骨架與外部 IK 目標端綁定單一 IK 約束
   <br>
   ![](moive/2023-03-18%2020_13_44.webp)
6. 將所有 IK 約束啟用 Stretch Compress，產生壓縮與伸展效果<br>手掌骨架繼承縮放關閉避免扭曲
   <br>
   ![](moive/2023-03-18%2020_24_36.webp)

## 多關節

![](moive/2023-03-20%2014_59_12.webp)

主要用的獸，或人體腳掌與腿的連接

> 不管是幾節，都可以套用此規則去延伸關節:
> + IK 末端點為父層級
> + 最後一節圖片骨架獨立調整旋轉

1. 建立符合圖片的骨架，並綁定對應的圖片
   <br>
   ![](moive/2023-03-20%2013_45_14.webp)
   ![](img/2023-03-20%2013_48_38.png)
2. 建立 IK 骨架，於圖片內12節與34節
   <br>
   ![](moive/2023-03-20%2013_45_24.webp)
3. 調整 IK 約束可伸縮<br>
   ![](moive/2023-03-20%2013_45_34.webp)
   ![](img/2023-03-20%2013_55_36.png)
   <br>調整 IK 末端點為父層級<br>
   ![](img/2023-03-20%2013_54_47.png)
   <br>調整圖片最末端骨架取消旋轉繼承<br>
   ![](img/2023-03-20%2013_54_58.png)
4. 建立動畫關鍵偵，符合動作運動
   <br>
   ![](moive/2023-03-20%2014_59_12.webp)
   ![](img/2023-03-20%2014_59_46.png)


## 參考

https://www.youtube.com/watch?v=mETraNnzuTg

https://www.youtube.com/watch?v=lVKb1Qq2I5g