# Spine 網格權重

負責修改圖片的網格與骨架的權重

1. [圖片網格(Mesh)](#圖片網格mesh)
2. [骨架權重(Weights)](#骨架權重weights)
3. [網格工具(Mesh Tools)](#網格工具mesh-tools)

## 圖片網格(Mesh)

![](img/2023-03-05%2017_25_52.png)
<br>
圖片使用 3D 網格進行動態活動

> 要啟用網格，選擇圖片後，`Tree`(人物層級)下方物件內容啟用`Mesh`後，點擊 `Edit Mesh`
> <br>
> ![](moive/2023-03-03%2017_32_00.webp)

![](img/2023-03-05%2017_29_29.png)
![](img/2023-03-05%2017_29_36.png)
<br>
網格工具可以使用的功能:

+ `Modify` - 修改，移動點/線，雙擊刪除
  <br>
  ![](moive/2023-03-03%2017_40_47.webp)
+ `Create` - 建立，插入點/線，雙擊刪除
  <br>
  ![](moive/2023-03-03%2017_50_00.webp)
+ `Delete` - 刪除，移除點/線
  <br>
  ![](moive/2023-03-03%2017_55_38.webp)
+ `New` - 新建，廢棄當前網格，重新拉線
  <br>
  ![](moive/2023-03-03%2018_04_09.webp)
+ `Reset` - 重置，廢棄當前網格，依據圖片最外圍建立四個線
  <br>
  ![](moive/2023-03-03%2018_39_22.webp)
+ `Genrate` - 細分，依據面細分點/線
  <br>
  ![](moive/2023-03-03%2018_42_43.webp)
+ `Trace` - 自動，依據透明度自動計算最外圍點/線
  <br>
  ![](moive/2023-03-03%2018_47_16.webp)
  <br>
  ![](img/2023-03-05%2017_40_17.png)
  ![](img/2023-03-05%2017_40_23.png)

## 骨架權重(Weights)

![](img/2023-03-04%2018_35_32.png)
![](img/2023-03-04%2018_35_42.png)
<br>
![](img/2023-03-04%2018_38_46.png)
![](img/2023-03-04%2018_38_57.png)

骨架對物件網格的控制權重
> 要先點擊 `Weights` 工具
> <br>
> 只對啟用 `Mesh` 的圖片有效
> <br>
> ![](img/2023-03-05%2017_46_49.png)
> ![](img/2023-03-05%2017_47_31.png)

+ 綁定骨架 - 對網格物件設置作用的骨架，第一次綁定會自動權重
  <br>
  ![](moive/2023-03-04%2015_40_09.webp)
+ 平滑權重 - 對選擇的點，平滑網格權重
  <br>
  ![](moive/2023-03-04%2015_46_18.webp)
+ 自動權重 - 對選擇的骨架與點，依據距離設置權重
  <br>
  ![](moive/2023-03-04%2015_50_29.webp)
  ![](img/2023-03-04%2016_05_35.png)
+ 修剪權重 - 對選擇的點依據閥值權重分配給其他骨架
  <br>
  ![](moive/2023-03-04%2016_02_31.webp)
+ 修改權重 - `Direct`(直接)/`Add`(增加)/`Remove`(減少)/`Replace`(覆蓋) 模式修改點的權重
  <br>
  ![](moive/2023-03-04%2018_42_13.webp)
  ![](img/2023-03-04%2017_56_58.png)
  ![](img/2023-03-04%2018_34_12.png)

網格權重顯示模式

+ `Pies` - 點的圓餅圖
  <br>
  ![](img/2023-03-04%2017_55_25.png)
+ `Overlay` - 骨架標記顏色，漸層附件
  <br>
  ![](img/2023-03-04%2017_55_36.png)
+ `Selected` - 只顯示選擇的骨架，用來搭配 `Pies` `Overlay`
  <br>
  ![](img/2023-03-04%2017_56_12.png)

## 網格工具(Mesh Tools)

用來範圍柔化操作網格的工具，可以用所有操作網格上
<br>
![](moive/2023-03-05%2015_31_50.webp)
<br>
![](img/2023-03-05%2017_03_57.png)
![](img/2023-03-05%2017_04_03.png)

+ `Size` - 範圍
+ `Feather` - 柔化範圍
+ `Hull vertices` - 啟用後不會超出最外圍的網格