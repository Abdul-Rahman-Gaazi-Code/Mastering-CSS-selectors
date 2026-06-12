- 1. The paragraph currently display the color Red,because of the #main-text ID selector. This comes down to CSS specificity, the weight system browsers use to decide which rule wins when multiple rules target the same element.ID selectors have the highest specificity of the three, so color red wins.

#

- 2. !important overrides the normal specificity system entirely,it sits above all regular rules. Even though both rules use the same #main-text ID selector (equal specificity), !important forces color green to win regardless.

#

- 3. p.highlight {color: green;}, This combines an element selector + class selector into one rule, giving it a specificity of 0-1-1 — higher than .highlight alone (0-1-0) or p alone (0-0-1). It still loses to the ID selector (1-0-0), but since we’re assuming the ID rule is removed from the picture for this scenario, this chained selector is the next strongest option.
#

  **Specificity is calculated like a 3-digit score: (IDs) — (Classes) — (Elements). The higher the score, the more “weight” a rule carries.​​​​​​​​​​​​​​​​**
