---
layout: post
title:  "ArchiCAD GDL Algorithm (1) - 泡沫排序法 Bubble Sort"
date:   2017-09-26 15:28:52 +0000
categories: jekyll update
---

![泡沫排序法](/assets/Algorithm/Bubble Sort/Bubble Sort.jpg)

# 樣板:    
<pre>
    <code>
! Create and initialize an array.
DIM array[6]
array[1] = 6
array[2] = 5
array[3] = 4
array[4] = 3
array[5] = 2
array[6] = 1

! Before using bubble sort, print the array.
x = 0
y = 0
gosub "PrintArray":

gosub "BubbleSort":

! After using bubble sort, print the array.
x = 0
y = -90/100
gosub "PrintArray":

! Subroutines
if 0 then
"PrintArray":
	for i = 1 to vardim1(array) 
		text2 x, y, str(array[i], 4, 0)
		x = x + 55/100
	next i
return

"BubbleSort":	
	for i = 1 to vardim1(array) - 1
		for j = 1 to vardim1(array) - i
			if array[j] > array[j + 1] then
				temp = array[j]
				array[j] = array[j + 1]
				array[j + 1] = temp
			endif
		next j
	next i
return

endif
    </code>
</pre>





[帶路雞Pro-App-Store]: https://appsto.re/tw/kp-Sfb.i
[帶路雞-App-Store]: https://appsto.re/tw/amD6eb.i

