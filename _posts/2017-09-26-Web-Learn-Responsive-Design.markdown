---
layout: post
title:  "Web Development 摘要 (1) Codecademy - Learn Responsive Design"
date:   2017-09-29 22:01:52 +0000
categories: jekyll update
---
By leafleafflower  

![泡沫排序法](/assets/Algorithm/Bubble Sort/Bubble Sort.jpg)

# 樣板:    
<Relative Mesurements>
Definition:
Content on a website can be sized relative to 
other elements on the page using relative mesurements.
-------------------------------------------------------

(unit)
em:  relative to the font size of a parent element
rem: relative to the font size of a root element <html>.

The unit of em sizes font relative to the font size 
of a parent element.

The unit of rem sizes font relative to font size of a
root element. That root element is the <html> element.
------------------------------------------------------------
(Percentage)
Sizing box-model features with percentage of their parent:
element
    width
    height
    borders
    padding
    margin

Percentages are commonly used to size box-model features,
like the width, height, borders, padding, margin of an
element.

When percentages are used to size width and height, child
elements will be sized relative to the dimensions of their
parent(remember that parent dimensions must first be set).

Percentages can be used to set padding and margin.
Horizontal and vertical padding and margin are set relative
to the width of a parent element.

-----------------------------------------------------------

(Width and Height - max and min)
min-width
max-width
min-height
max-height

(Width adn Height - proportionally)
Width or height is set, and the other is set auto.

(Background Image - proportionally)
background-image: url('camel-background.png');
background-position: center;
background-repeat: no-repeat;

background-size: cover; /* scale proportionally */


The minium and maximum width of elements can be set
using min-width and max-width.

The minium and maximum height of elements can be set
using min-height and max-height.

When the height of an image or video is set, then its
width can be set to auto so that the media scales 
proportionally.
Reversing these two properties and values will also 
achieve the same result.

A background image of an HTML element will scale
proportionally when its background-size property is set
to cover.

(Use)
Relative units of measurement are a first step towards
incorporating responsive techniques, you can create a
seamless user experience regardless of a device's screen
size.

<Media Queries>

Definition:
When a website responds to the size of the
screen it's viewed on, it's called a responsive
design.

Use:
You can write media queries to help with
different screen sizes.
-------------------------------------------------
動作：media queries
條件：media features
條件and：and
條件or ：,(comma)
找需要設條件的地方：調整瀏覽器大小找斷點
學會media query的好處：讓用戶在各種螢幕尺寸上，
                     都有良好的觀看體驗


Media queries require media features.
Media features are the conditions that must
be met to render the CSS within a media query.

Media features can detect many aspects of 
a user's browser, including the screen's
width, height, resolution, orientation, and
more.

The and operator requires multiple media
features to be true at once.

A comma separated list of media features
only requires onew media feature to be true
for the code within to be applied.

The best practice for identifying where
media queries should be set is by resizing
the browser to determine where the content naturally
breaks. Natural breakpoints are found by resizing
the browser.

--------------------------------------------------
With your knowledge of media queries and CSS, 
you can make websites that look great on 
any device, from a small phone to a huge 
television. By making your websites responsive, 
you'll make it possible for any of your users to 
have a great experience.






[帶路雞Pro-App-Store]: https://appsto.re/tw/kp-Sfb.i
[帶路雞-App-Store]: https://appsto.re/tw/amD6eb.i

