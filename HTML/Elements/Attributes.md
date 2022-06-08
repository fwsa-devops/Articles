# Attributes

An Attribute extends an HTML and XML element, changing its behavious or providing metadata.

An attribute always has the form name="value" (the attribute's identifier followed by its associated value).

You may see attributes without the equals sign or a value. That is a shorthand for providing the empty string in HTML, or the attribute's name in XML.

```html
<input required>
<!-- is the same as… -->
<input required="">
<!-- or -->
<input required="required">
```

## Global Attributes

Global attributes are attributes common to all HTML elements; they can be used on all elements, though they may have no effect on some elements.

Global attributes may be specified on all HTML elements, even those not specified in the standard. That means that any non-standard elements must still permit these attributes, even though using those elements means that the document is no longer HTML5-compliant. For example, HTML5-compliant browsers hide content marked as <foo hidden>...</foo>, even though <foo> is not a valid HTML element.

### few of the Global Attributes are :

- `id`
- `class`
- `type`
- `required`
- `minlength`
- `maxlength`
- `min`
- `max`
- `autofocus`
