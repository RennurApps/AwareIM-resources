Element: Business Object
Area: Form
Advanced Script: Render
Attribute: Plain Text 
Script: 
var f = parser.getField ("ColorAttrName");
$("#" + f.getId ()).kendoColorPicker ({
value: f.getValue (),
buttons: false,
change: function (e) {
f.setValue (e.value);
}
});
