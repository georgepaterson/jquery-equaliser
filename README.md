# [jQuery Equaliser plugin](http://www.georgepaterson.com)

Equalises the vertical height and position of an array of HTML elements within a given parent element.

## Dependencies

Requires [jQuery](http://jquery.com/)  1.4 +


## Supported Browsers

Internet Explorer 6 +

Current versions of:

Firefox
Safari
Chrome
Opera

## Plugin parameters

* columns: Number of columns in the group, default 'auto', can be set to an integer.
* rows: Number of rows in the group, default 'auto', can be set to an integer.
* equalise: The elements in the group to equalise position, an array of classnames and tag names.
* equaliseMethod: The method to equalise position, uses standard CSS construct. Defaults to 'margin-top', could be 'padding-top'.
* setHeight: Boolean value, whether of not equalise the height of the groups child containers.

## Usage

Simple equal heights.

	<ul id="example-one">
		<li>
			<p>Lorem ipsum dolor.</p>
		</li>
		<li>
			<p>Lorem ipsum dolor sit amet.</p>
		</li>
		<li>
			<p>Lorem ipsum.</p>
		</li>
		<li>
			<p>Lorem ipsum dolor sit.</p>
		</li>
	</ul>

	<script>
	  	$(document).ready(function() {
			$('#example-one').equaliser();
		});
	</script>

Equal heights with .example vertically positioned equally.

	<ul id="example-two">
		<li>
			<p>Lorem ipsum dolor.</p>
			<p class="example">Lorem ipsum.</p>
		</li>
		<li>
			<p>Lorem ipsum dolor sit amet.</p>
			<p class="example">Lorem ipsum.</p>
		</li>
		<li>
			<p>Lorem ipsum.</p>
			<p class="example">Lorem ipsum.</p>
		</li>
		<li>
			<p>Lorem ipsum dolor sit.</p>
			<p class="example">Lorem ipsum.</p>
		</li>
	</ul>

	<script>
	  	$(document).ready(function() {
			$('#example-one').equaliser({equalise: ['.example']});
		});
	</script>

## Links

* Author:	[George Paterson](http://www.georgepaterson.com)
* Company:	[LBi](http://lbi.co.uk)
* Demo:		[jQuery Equaliser plugin](http://www.georgepaterson.com)
* Source:	[Github](http://github.com/georgepaterson/jquery-equaliser)

## License

Copyright 2011, [George Paterson](http://www.georgepaterson.com)

Dual licensed under the MIT or GPL Version 2 licenses.
	
Please use the [GitHub issue tracker](http://github.com/georgepaterson/jquery-equaliser/issues) for bug reports and feature requests.
