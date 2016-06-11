## Topics
1. xpath in your browser
2. find and replace
3. FLOWR expressions
4.

## Setup
http://basex.org/products/download/
Mac: brew install basex
Windows: use installer
Linux: use distribution

In your terminal, run

```$ basexgui```

## Introduction
xpath
xslt

## Exercise

* xpath terms syntax
* Edit a document and a collection
* flowr expression - group by
* isolating certain elements
* Edit a collection database, grouping by name, count, bring back snippets
GOAL: generate a report

* replace and insert update delete
GOAL: clean up a collection

BONUS
IN-BROWSER XPATH
http://code4libtoronto.github.io/librarycarpentry20160728/
Inspect
$x(".//p[@id='who']")
$x(".//p[@id='who']/text()")
https://getfirebug.com/wiki/index.php/$x
$x(".//*/a")
$x(".//*//a")

## Glossary
node, root, descendent, parent, ancestor, context, element, attribute, namespace, axis
