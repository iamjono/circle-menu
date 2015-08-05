Circle Menu
===========

A customizable jQuery plugin that emulates the menu in the [Path][] application.  Includes a 
selection animation and various animation options for opening and closing the menu.

**[See it in action.][demo]**

**[Read the Documentation.][docs]**

**Compatibility:**

Fully Working:

* Chrome
* Firefox
* Android
* Opera

Known Issues:

* IE 9 
  * Does not include CSS animations for open/close, as it does not support CSS transitions.

Repository forked
=======================
This repository has been forked to provide a custom addition - the ability to offset each element by a specific number of pixels per index. Useful for creating a linear menu like this:

```
		$('#wheelnav-wide').circleMenu({
			circle_radius: 50,
			item_diameter: 46,
			angle:{start:90, end:90},
			trigger:'click',
			step_out:-60,
			offset_y: 100,
			select: function(){$('#wheelnavcontroller').removeClass('rotated45')},
			open: function(){$('#wheelnavcontroller').addClass('rotated45')},
			close: function(){$('#wheelnavcontroller').removeClass('rotated45')}
		});
```

[Path]: https://path.com/
[demo]: http://zikes.github.com/circle-menu/examples/
[docs]: http://zikes.github.com/circle-menu/
