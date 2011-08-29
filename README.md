What is it?

The TickerType jQuery plugin allows you to animate a set of headlines or any other list of text items.

How do I use it?

To implement, simply include the latest jquery library as well as jquery.tickertype.js in the `<head>` tag of your HTML page

	<head>
	  <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
	  <title>jquery.tickertype - Demo</title>
	  <link href="tickertype.demo.css" rel="stylesheet" type="text/css" />
	  <script type="text/javascript" src="jquery-1.2.6.min.js"></script>
	  <script type="text/javascript" src="jquery.tickertype.js"></script>
	</head>
Next, add a `<div>` tag and set the id attribute to ticker-area. Within this `<div>` tag, create an unordered list of the text fragments you would like to be display in the ticker. List items may include simple HTML tags, such as links, `<strong>` and `<em>`.

	<div id="ticker-area">
	  <ul>
	    <li>Sed venenatis <a href="http://www.google.com">diam quis</a> lorem. Curabitur.</li>
	    <li>Fusce <strong>vehicula</strong> iaculis felis. Phasellus congue!</li>
	    <li>Morbi vitae enim vel <em>purus sollicitudin</em>.</li>
	  </ul>
	</div>
	
The code above will rotate through the 3 items endlessly. If you would like the ticker to stop animating after a number of cycles, simple at alt="2" to the ticker-area div tag, substituting the number of cycles you would like before animation stops. After the animation stops, the last item in the set will remain on he screen. For example:

	<div id="ticker-area" alt="10">
	  <ul>
	    <li>Sed venenatis <a href="http://www.google.com">diam quis</a> lorem. Curabitur.</li>
	    <li>Fusce <strong>vehicula</strong> iaculis felis. Phasellus congue!</li>
	    <li>Morbi vitae enim vel <em>purus sollicitudin</em>.</li>
	  </ul>
	</div>

The code above will rotate through the 3 items 10 times and then stop on the last item.