#Target Attribute
## \<base target="\_value"\>
You can set the default handling of clicked hyperlinks & forms within each document by:
```html
<base target="_value">
```

Basically: How a link opens.

When no value is set, it will be set to
```html
<base target="_self">
```

Common options:
>	\_blank: New tab/window\
>	\_self: Current frame\*

Obsolete options**:
>	\_parent: Parent frame\
>	\_top: Full body of window\
>	*framename*: Replace with preferred frame's name

\* *Used 'frame' due to the information following up.*\
\*\* Only useable with iframes, since frames & framesets are no longer supported.

*(Personal opinion: Avoid the use of iframes)*

## Override base setting
The base set is only to set the document's default value.
You can override the base setting by using the target attribute for individual hyperlinks/forms.

Example hyperlink usage:
```html
<a href="example.html" target="_blank">
```

Example form usage:
```html
	<form action="/example.php" method="post" target="_blank">
		Input text:
		<input type="text" name="txt1"><br />

		Select option:
		<select>
			<option value="opt1">Example 2</option>
			<option value="opt2">Example 2</option>
		</select>

		<input type="submit" value="Submit">
	</form>
```
