- 1. nth-child(2) targets the element that is the 2nd child of its parent. Since all three "li>" items share the same parent "ul>", this precisely hits “Item 2” only.

#

- 2. The second "p>" is the very last element inside .container, so :last-child target it.

#

- 3. A descendant selector targets any "p>" that lives anywhere inside .container, which is exactly both of them.

#

**Challenge**

- 4. Because :nth-child() doesn’t mean “the first paragraph.” It means “an element that is both a "p>" and the 1st child of its parent. But looking at the actual child order inside .container it is not right.The first "p>" is the 2nd child, not the 1st that spot is taken by "h2>". So p:nth-child(1) finds nothing, because no element can simultaneously be a "p>" and the 1st child here.
