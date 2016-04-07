# Integration of color picker

## Source
 - [Aware IM Forum](http://www.awareim.com/forum/viewtopic.php?f=1&t=8588)
 - Kendo UI Widget: [kendoColorPicker demo](http://demos.telerik.com/kendo-ui/colorpicker/index) 

## Business Object Form
 - Element: **Business Object** <br>
 - Area: **Form** <br>
 - Advanced Script: **Render** <br>
 - Attribute: **Plain Text** <br>
 - Attribute Name: **_ColorAttrName_** <br>
 - **Aware IM Script**: <br>
 var f = parser.getField ("**_ColorAttrName_**");<br>
 $("#" + f.getId ()).kendoColorPicker ({ <br>
value: f.getValue (), <br>
buttons: false, <br>
change: function (e) { <br>
f.setValue (e.value); <br>
} <br>
}); <br> 

## Query Grid 

#### No Inline Editing 
 - Advanced Script: **Initialization** 
 - **Aware IM Script**: <br>
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

#### Inline Editing 
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

return value; <br>
}; <br>
c.editor = function(container, options) { <br>
var input = $("<input/>");<br>
input.attr("name", options.field);<br>
input.appendTo(container);<br>
input.kendoColorPicker({<br>
buttons: false<br>
});<br>
}<br>
}<br>
}<br>
