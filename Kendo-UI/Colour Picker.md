# Integration of color picker
## Business Object Form
 - [Source](http://www.awareim.com/forum/viewtopic.php?f=1&t=8588)
 - Element: **Business Object** <br>
 - Area: **Form** <br>
 - Advanced Script: **Render** <br>
 - Attribute: **Plain Text** <br>
 - Attribute Name: **_ColorAttrName_** <br>
 - Aware IM Script: <br>
 var f = parser.getField ("**_ColorAttrName_**");<br>
 $("#" + f.getId ()).kendoColorPicker ({ <br>
value: f.getValue (), <br>
buttons: false, <br>
change: function (e) { <br>
f.setValue (e.value); <br>
} <br>
}); <br> 
 - Kendo widget: [kendoColorPicker demo](http://demos.telerik.com/kendo-ui/colorpicker/index) 
## Query Grid
 - Advanced Script: **Initialization** 
 - Script: <br>
 for (var i = 0; i < config.columns.length; ++ i) <br>
{<br>
var c = config.columns[i];<br>
if (c.field == "ColorAttrName")<br>
{<br>
var old = c.template;<br>
c.template = function (dataItem) {<br>
var value = old (dataItem);<br>
if (value)<br>
{<br>
return "<div style='background-color:" + value + ";width:100px;height:20px;'></div>";<br>
} <br>
return value;<br>
};<br>
}<br>
}<br>
