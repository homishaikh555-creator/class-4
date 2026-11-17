CSS BOX MODEL ASSIGNMENT
========================

Files included
--------------
index.html : Contains the webpage structure and box model examples.
style.css  : Contains the styles, widths, heights, padding and borders.
README.txt : This written explanation.

How to run
----------
1. Extract the ZIP file.
2. Keep index.html and style.css in the same folder.
3. Open the folder in Visual Studio Code.
4. Open index.html in Chrome (or use VS Code Live Server).

Written description
-------------------
The CSS Box Model explains how the browser calculates the size of an HTML
element. It has four parts:

1. Content: The text, image or other material inside the element.
2. Padding: Space between the content and the border.
3. Border: The line around the padding and content.
4. Margin: Space outside the border, separating the element from others.

Width experiment
----------------
Box A:
Content width = 200px; left and right padding = 10px each;
left and right border = 2px each.
Total width = 200 + 20 + 4 = 224px.

Box B:
Content width = 200px; left and right padding = 25px each;
left and right border = 5px each.
Total width = 200 + 50 + 10 = 260px.

Box C:
Declared width = 200px with box-sizing: border-box.
The 200px includes content, padding and border, so the content area is
smaller than 200px.

Height experiment
-----------------
Height A:
Content height = 100px; top and bottom padding = 10px each;
top and bottom border = 2px each.
Total height = 100 + 20 + 4 = 124px.

Height B:
Content height = 100px; top and bottom padding = 25px each;
top and bottom border = 5px each.
Total height = 100 + 50 + 10 = 160px.

Height C:
Declared height = 160px with box-sizing: border-box.
The 160px includes content, padding and border.

Conclusion
----------
With content-box (the default CSS sizing model), declared width and height
apply to the content only. Padding and border are added outside them.

With border-box, declared width and height include content, padding and
border. This makes it easier to control the final size of elements.

Margin is outside the border and is not included in these width/height
calculations.
