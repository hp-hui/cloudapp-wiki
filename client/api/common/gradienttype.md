## GradientType

* string
	* &lt;type: linear&gt; &lt;direction: top|bottom|left|right|top-left|bottom-right|top-right|bottom-left&gt; [ColorType](colortype.md) [ColorType](colortype.md) ...
* table
	```
	{
	    mode = "linear",
	    coordinate = {
	        startX, startY,
	        endX, endY
	    },
	    color = {
	        ColorType, ColorType, ...
	    }
	}
		```
