# Barcode39 v0.0.1
# How to use

```
	<script>
		new Barcode39;
	</script>
```

Thats it!

## API

#### BarCode39@toString
- Prints out the string that drew the barcode
```
	<script>
		var b = new Barcode39;
		b.toString() // the content of your element
	</script>
```

#### BarCode39@toDataURL
- Prints out the Data URL
```
	<script>
		var b = new Barcode39;
		b.toDataURL() // data:image/png;base64,*
	</script>
```

#### BarCode39@toBarcode
- Prints out the Data URL
```
	<script>
		var b = new Barcode39;
		b.toBarcode() // [BwbwbWBwb]w[BwbwbWBwb]w[etc...]
	</script>
```

## Barcode39 Parameters

```
	<script>
		var b = new Barcode39(elementId, type, delimeter);
	</script>
```
#### @elementId
- The element to grabs its value from

#### @type
- The type of which to display (doesnt matter what type, its all for the toBarcode method)
- Look at formats here: http://en.wikipedia.org/wiki/Code_39

#### @delimeter
- The standard for wrapping barcode text values is "*" but you can change this

## Barcode39 HTML

Barcode39 needs an element to create an image element within.

By default, the element Barcode39 looks for is an element with an ID of "barcode"

```
	<div id="barcode"></div>
```

We also need to provide a value to code, otherwise Barcode39 will throw an error.

```
	<div id="barcode">123123123123123123123123</div>
```

All non-recognizable characters are turned into "-".

Have fun!

# Support

I'm only supporting browser with canvas. I havent tried ex-canvas with this yet, but it should work...

Patches and pulls are more than welcome!

# The MIT License (MIT)
Copyright © 2012-2013 Erik Zettersten

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.