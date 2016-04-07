Element: **Business Object** <br>
Area: **Form** <br>
Advanced Script: **Render** <br>
Attribute: **Plain Text** <br>
Script: <br>
<quote>var f = parser.getField ("**ColorAttrName**");
$("#" + f.getId ()).kendoColorPicker ({
value: f.getValue (),
buttons: false,
change: function (e) {
f.setValue (e.value);
}
});
</quote>
