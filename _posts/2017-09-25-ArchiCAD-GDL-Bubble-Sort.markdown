---
layout: post
title:  "ArchiCAD GDL Algorithm (1) - 泡沫排序法 Bubble Sort"
date:   2017-09-25 13:50:52 +0000
categories: jekyll update
---

![柱磁磚計畫物件說明](/assets/Algorithm/Bubble Sort/Bubble Sort.jpg)

# 物件描述:  
> 物件使用在柱子使用兩邊整磚，中間切磚的排磚法。相比之前的排磚方法，各種又磨又切的尺寸，數量難以計算，這種排磚法可以讓數量計算單純化，磨角的尺寸只剩下一種整磚，切磚的尺寸也只有一種，在數量變單純的同時也兼顧了美觀。
<code>
DIM array[6]
array[1]=6
array[2]=5
array[3]=4
array[4]=3
array[5]=2
array[6]=1


x = 0
y = 0
gosub "PrintArray":
gosub "BubbleSort":

x = 0
y = -90/100
gosub "PrintArray":

if 0 then
"PrintArray":
	for i=1 to vardim1(array) 
		text2 x, y, str(array[i], 4, 0)
		x = x + 55/100
	next i
return
"BubbleSort":	
	for i=1 to vardim1(array) - 1
		for j=1 to vardim1(array) - i
			if array[j] > array[j + 1] then
				temp = array[j]
				array[j] = array[j + 1]
				array[j + 1] = temp
			endif
		next j
	next i
return

endif

<code/>


# 依寬度自動排列磁磚:
![自動排列](/assets/ColumnTileWork/ColumnTileworkAutoArrangement.jpg)



[帶路雞Pro-App-Store]: https://appsto.re/tw/kp-Sfb.i
[帶路雞-App-Store]: https://appsto.re/tw/amD6eb.i

