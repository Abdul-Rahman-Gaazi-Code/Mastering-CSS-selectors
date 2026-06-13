
**Scenario A**
- The color of the text is blue.
#
- Both rules applies to the "p>":
	∙	* directly targets it and sets color to orange (specificity: 0-0-0)
	∙	div targets its parent and sets the div’s color to blue.
    "*" directly targeted element always beats an inherited value — even if the direct rule has lower specificity.
    * directly targets the "p>" with color: orange. But div { color: blue } sets blue on the parent, and since color is an inherited property, the "p>" would naturally inherit blue  except * is already directly targeting it with orange.