Selectivizr
-----------

**CSS3 selectors for IE 6-8**

A custom build that gets round the IE8 XDomainRequest issue of it needing xhr.onload to get the file contents and having to wait for this to finish each time we call a file. 

// Still need to allow for more than one media query but it works for one :)


_selectivizr_ is a JavaScript utility that emulates CSS3 pseudo-classes
and attribute selectors in Internet Explorer 6-8. Simply include the
script in your pages and selectivizr will do the rest.

To use the library, you'll need to include one of the supported libraries:

  * jQuery (1.3+)
  * Dojo (1.5.0+)
  * Prototype (1.6.1+)
  * Yahoo UI Library (2.8.0+)
  * DOMAssistant (2.8.0+)
  * MooTools (1.3+)
  * NWMatcher (1.2.3+)
  
Then add the following conditional comment _AFTER_ your stylesheets:

	<!--[if (gte IE 6)&(lte IE 8)]>
	  <script type="text/javascript" src="selectivizr.js"></script>
	  <noscript><link rel="stylesheet" href="[fallback css]" /></noscript>
	<![endif]-->

This adds the `selectivizr.js` and an optional fallback CSS file to IE6-8 while
hiding for other browsers.
