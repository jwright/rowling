rowling
=======

## DESCRIPTION

A client side editor to turn table rows into an editable row. Inspired by [rest-in-place](https://github.com/janv/rest_in_place) with support for multiple fields and different forms.

## USAGE

```
$(".my-table tr").rowling({
  url: "/resource/123",
  objectName: "resource",
  method: "put",
  attributes: [
    "attribute1",
    "attribute2"
  ],
  formType: [
    { "attribute1": "input" },
    { "attrubute2": "textarea" }
  ], // alternatively formType: "row", or formType: "http://localhost:3000/my-form"
  activate: function() { },
  ready: function() { },
  update: function() { },
  success: function() { },
  abort: function() { }
});
```
