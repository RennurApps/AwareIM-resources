# Integration of color picker on a form [Source](http://www.awareim.com/forum/viewtopic.php?f=1&t=8588)
 - Element: **Business Object** <br>
 - Area: **Form** <br>
Advanced Script: **Render** <br>
Attribute: **_ColorAttrName_** **Plain Text** <br>
Script: <br>
 var f = parser.getField ("**_ColorAttrName_**");<br>
 $("#" + f.getId ()).kendoColorPicker ({ <br>
value: f.getValue (), <br>
buttons: false, <br>
change: function (e) { <br>
f.setValue (e.value); <br>
} <br>
}); <br>
