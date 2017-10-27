---
layout: post
title:  "【ARCHICAD GDL】GDL的測試驅動開發"
date:   2017-10-25 22:01:52 +0000
categories: jekyll update
---
By leafleafflower  
![TDD](/assets/ArchiCAD/TDD.png)  

# 樣板:    
<pre>
    <code>
! Red
! Green
! Refractor
define style "widthDimensioningStyle" textfont, textHeight*1000, 5, 0

addY 10/100
prefix = "testAdder(11 + 22 = 33)"
a = 11
b = 22
expected = 33
gosub "adder":
result = returnValue
gosub "assert":

addY 10/100
prefix = "testAdder(110 + 22 = 132)"
a = 110
b = 22
expected = 131
gosub "adder":
result = returnValue
gosub "assert":


if 0 then
"adder":
	returnValue  = a + b
return

"assert":
	successExpression  = "success"
	failExpression = "fail"

	if expected = result then
		material 76 ! green

		! TEXT d, 0, expression
		!define style "widthDimensioningStyle" textfont, textHeight*1000, 5, 0
		set style "widthDimensioningStyle"
		
		text 0,0, prefix + " " + successExpression

	else
		material 19 ! red

		! TEXT d, 0, expression
		!define style "widthDimensioningStyle" textfont, textHeight*1000, 5, 0
		set style "widthDimensioningStyle"
		
		text 0,0, prefix + " " + failExpression
	endif
return

endif

    </code>
</pre>





-------------------------------------------------------  

[帶路雞Pro-App-Store]: https://appsto.re/tw/kp-Sfb.i
[帶路雞-App-Store]: https://appsto.re/tw/amD6eb.i

