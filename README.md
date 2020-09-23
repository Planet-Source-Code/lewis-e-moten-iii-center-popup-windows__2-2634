<div align="center">

## Center Popup Windows


</div>

### Description

Center popup windows in the middle of your browser.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Lewis E\. Moten III](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/lewis-e-moten-iii.md)
**Level**          |Advanced
**User Rating**    |3.1 (25 globes from 8 users)
**Compatibility**  |
**Category**       |[Alerts & Prompts](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/alerts-prompts__2-85.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/lewis-e-moten-iii-center-popup-windows__2-2634/archive/master.zip)





### Source Code

```
<SCRIPT>
function getbrowserwidth()
{
	if (navigator.userAgent.indexOf("MSIE") > 0)
	{
		return(document.body.clientWidth);
	}
  else
  {
		return window.outerWidth;
	}
}
function getbrowserheight()
{
	if (navigator.userAgent.indexOf("MSIE") > 0)
	{
		return(document.body.clientHeight);
	}
  else
  {
		return(window.outerHeight);
	}
}
var popup = new Object()
function CenterPopup(URL, width, height)
{
	// get center of browser window
	var X = getbrowserwidth() / 2
	var Y = getbrowserheight() / 2
	popup = window.open(URL, 'PopUp',
		'scrollbars=yes ' +
		'width=' + width + ' ' +
		'height=' + height + ' ' +
		'top=' + (window.screenTop + (Y - (height/2))) + ' ' +
		'left=' + (window.screenLeft + (X - (width/2)))
		)
	popup.focus()
}
</SCRIPT>
<A href="" onclick="CenterPopup('http://www.lewismoten.com/', 640, 480);return(false);">PopUp</A>
```

