# Spine 人體骨盆

演示如何製作立體移動的骨盆關節

> 製作重點:骨架層級牽動與變換約束正負數

## 骨盆製作

1. 建立骨架層級
   <br>
   ![](moive/2023-03-19%2010_58_19.webp)
   ![](img/2023-03-19%2011_00_03.png)
2. 建立骨盆的 IK 約束
   <br>
   ![](moive/2023-03-19%2010_58_29.webp)
4. 連接骨盆與控制端的變換約束
   <br>
   ![](moive/2023-03-19%2010_58_39.webp)
   <br>
   ![](img/2023-03-18%2023_48_22.png)
   ![](img/2023-03-18%2023_48_28.png)

骨架層級不同與變換數值類型如下:

|      約束      |使用|                 演示                  |
| :------------: |:---:| :-----------------------------------: |
|   IK + 變換    |圖形邊形| ![](moive/2023-03-18%2023_33_21.webp) |
|      變換      |端點骨架| ![](moive/2023-03-18%2023_33_31.webp) |
| 變換(數值差異) |前後距離| ![](moive/2023-03-18%2023_33_41.webp) |

## 人體臀部

![](moive/2023-03-18%2023_31_15.webp)

1. 建立骨架層級符合圖片
   <br>
   ![](moive/2023-03-19%2017_55_15.webp)
   ![](img/2023-03-19%2020_16_37.png)
2. 骨架綁定圖片權重
   <br>
   ![](moive/2023-03-19%2017_55_25.webp)
3. 建立控制器，並綁定骨架
   <br>
   ![](moive/2023-03-19%2017_55_35.webp)
4. 建立 IK 控制腳步
   <br>
   ![](moive/2023-03-19%2017_55_45.webp)
5. 設走路動畫關鍵值
   <br>
   ![](moive/2023-03-19%2017_55_55.webp)
   ![](img/2023-03-19%2018_36_26.png)

## 生動臀部

![](moive/2023-03-19%2019_50_46.webp)

生動臀部主要在動作符合人體規律，圖片有晃動感，不能破圖

+ 網格依據圖片，骨架權重依據動作調整
  <br>
  ![](img/2023-03-18%2023_05_10.png)
  ![](img/2023-03-18%2023_05_21.png)
  ![](img/2023-03-18%2023_05_39.png)
+ 圖片添加晃動的控制端
  <br>
  ![](moive/2023-03-19%2019_50_26.webp)
+ 身體添加搖晃
  <br>
  ![](moive/2023-03-19%2019_50_36.webp)
  ![](img/2023-03-19%2020_16_55.png)
+ 調整動畫關鍵偵，如:人體在移動時，踏腳那邊臀部會用力抬高
  <br>
  ![](img/2023-03-19%2020_11_02.png)

## 參考來源

https://www.youtube.com/watch?v=gjGmCWL4ICE