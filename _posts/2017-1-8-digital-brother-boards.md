---
layout: post
title:  "Digital Brother Boards"
date:   2017-1-8 20:41:00 -0800
tagline: In which abstraction helped make sense of other abstraction
---
# TODO link to DBB

Google Orgchart? Nope.

d3.js? Sure, why not?

Implementing my own algorithm to draw trees in SVG without overlapping nodes/links, with non-constant link lengths? Nooope.

Enter the wonderful work of [Jason Davies][jason-davies]--namely his [Tree of Life][tree-of-life], which is built on a small JavaScript library of his called newick.js.

I derived the context-free grammar for Newick format as follows:
- *S* -> a
- *S* -> (*A*)a
- *A* -> *A*:n
- *A* -> *A*,*A*

where a is the name of some node, and n is the distance from a to its parent. Breaking it down like this allowed me to create a (very ugly) almost-one-liner function to convert an array of brother objects in JSON to Newick format.

```javascript
writeNewickString(brother) {
	let hisLittles = this.getLittles(brother);
	let nodeRepresentation = someBrother => someBrother.brotherNumber + (!someBrother.bigBrotherNumber ? '' : ':' + this.getBigDistance(someBrother));
	return !hisLittles.length ? nodeRepresentation(brother) : '(' + hisLittles.map(someBrother => this.writeNewickString(someBrother) ).join(',') + ')' + nodeRepresentation(brother);
}
```

[jason-davies]: https://twitter.com/jasondavies
[tree-of-life]: https://www.jasondavies.com/tree-of-life/