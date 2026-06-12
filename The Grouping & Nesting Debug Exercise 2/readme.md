- 1. Nav a means any "a" that lives somewhere inside "a <nav>” nothing outside is affected.

#

- 2. h2 h3 doesn’t mean “h2 and h3.” It means “an h3 nested inside an h2” which never exists in valid HTML. So this rule matches nothing,The comma is what tells CSS “apply this rule to both of these separately.

#

- 3. Both "ul class="main-list" elements (in "nav" and in "section")" have the same structure their "li>" items are all direct children with no nesting. So ">" correctly bolds only those direct children in both lists, and would stop working if someone added a nested "ul" inside an "li" later on.
