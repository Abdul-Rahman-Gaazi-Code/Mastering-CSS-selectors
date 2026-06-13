**Scenario A**

- The color of the text is blue.

#

- Both rules applies to the "p>":
  ∙ _ directly targets it and sets color to orange (specificity: 0-0-0)
  ∙ div targets its parent and sets the div’s color to blue.
  "_" directly targeted element always beats an inherited value even if the direct rule has lower specificity.
  - directly targets the "p>" with color: orange. But div { color: blue } sets blue on the parent, and since color is an inherited property, the "p>" would naturally inherit blue except \* is already directly targeting it with orange.

#

**Scenario B**

- The "p>" displays green.

* directly targets the paragraph with purple at specificity 0-0-0. .highlight also directly targets it with green at specificity 0-1-0. Both rules are in direct competition same element, same property. Specificity decides,The universal selector has zero specificity any class, ID, or element selector will always beat it in a direct conflict.
