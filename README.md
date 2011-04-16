# [jQuery Equaliser plugin](http://www.georgepaterson.com)

Equalises the vertical height and position of an array of HTML elements within a given parent element.

## Dependencies

Requires [jQuery](http://jquery.com/)  1.4 +

## Supported Browsers

* Firefox 2.0+
* Internet Explorer 6+
* Safari 3+
* Opera 9+
* Chrome 1+

## Plugin parameters

* columns: Number of columns in the group, default 'auto', can be set to an integer.
* rows: Number of rows in the group, default 'auto', can be set to an integer.
* equalise: The elements in the group to equalise position, an array of classnames and tag names.
* equaliseMethod: The method to equalise position, uses standard CSS construct. Defaults to 'margin-top', could be 'padding-top'.
* setHeight: Boolean value, whether of not equalise the height of the groups child containers.

## Usage

Each direct child element of the should be vertically spaced by some method. 

Commonly this can be performed by the CSS styles `float: left` and `display: inline-block`.

Unordered list only used as a semantic method, HTML structure can be formed differently.

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
			$('#example-two').equaliser({equalise: ['.example']});
		});
	</script>

---
	
Please use the [GitHub issue tracker](http://github.com/georgepaterson/jquery-equaliser/issues) for bug reports and feature requests.
