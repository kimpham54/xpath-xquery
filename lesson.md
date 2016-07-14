https://digital.library.yorku.ca/yul-95212/hairdressing-mr-gino-bay-beauty-salon/datastream/MODS/view
https://digital.library.yorku.ca/yul-93087/dog-obedience-course-lawrence-plaza/datastream/MODS/view
http://digitalscholarship.utsc.utoronto.ca/projects/islandora/object/nearbystudies%3A546/datastream/MODS/view
http://digitalscholarship.utsc.utoronto.ca/projects/islandora/object/nearbystudies%3A585/datastream/MODS/view

## Topics
1. xpath in your browser
2.
3. FLOWR expressions, querying order or grouping
4. functions https://www.w3.org/TR/xpath-functions-30/
find and replace
xquery update

## Setup
http://basex.org/products/download/
Mac: brew install basex
Windows: use installer
Linux: use distribution

In your terminal, run

```$ basexgui```

Database > New
From a folder, name your database

## Introduction
Introduction to XPath
XPath (which stands for XML Path Language) is an expression language used to specify parts of an XML document, which is designed to be used by XML tooling languages such as XSLT or XQuery. XPath is also used in HTML like jQuery. Called 'path' because uses notations like URLS or unix directories

XSLT - a language for transofrming XML documents into other documents (XML, HTML, etc)
XQuery - a language for querying and programming XML documents

Why is it useful?
XPath is written using expressions, expressions when evaluated will produce an object. Typically used to select nodes, compare nodes, ? but technically you can't produce a node or list of nodes? Use XQuery for that

What does an XPath expression evaluate to?
node-set
boolean
number
string

What is it evaluated against?
A context (context node)


BUILDING AN EXPRESSION
Anatomy of a Location Step

child:: list [count(descendent::item) > 8]

Each location step has at least two parts (may have three)

An axis ( child:: )
Where are you going (in relation to the evaluation context)?
A node test (the name of an element “ list ”)
What kind of node do you want?
Zero or more predicates [count(descendent::item) > 8]
What other conditions must be true of these nodes?
Location Step = axis:: + nodetest + [predicate]*


## Exercise

* xpath terms syntax
* Edit a document
* Edit a collection
* flowr expression - group by
* isolating certain elements
* Edit a collection database, grouping by name, count, bring back snippets
* chaining variable assignment
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

xpath tree google images

## Glossary
node, root, descendent, parent, ancestor, context, element, attribute, namespace, axis

## Links
https://www.w3.org/TR/xpath-31/
http://www.wwp.northeastern.edu/outreach/seminars/sc2013/presentations/xslt/xml_and_xpath_00.xhtml
http://www.mulberrytech.com/papers/XPath-2-0-User-Grp-HTML/contents.html
http://www.xmlmind.com/tutorials/XQueryUpdate/#d0e41
http://docs.basex.org/wiki/XQuery_3.0#String_Concatenations
http://gvwilson.github.io/new-lesson-example/
https://www.steffanick.com/adam/blog/convert-csv-to-xml-with-xquery/
https://docs.google.com/document/d/1oWXD5eE7BMXuEx4cLEqrenOiWIhmcJCWLzPKHMHbGgU/edit
https://www.google.ca/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=basex+xquery+collection
http://edutechwiki.unige.ch/en/XQuery_tutorial_-_basics#FLWOR_expressions
gists github
http://www.brainbell.com/tutorials/XML/Understanding_XPath.htm


return vs return element
