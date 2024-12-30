---
title: "DITA XML Reference Guide"
date: 2023-02-10
categories:
  - blog
tags:
  - technical writing
  - DITA
  - XML
---

A quick reference guide on Darwin Information Typing Architecture (DITA) elements.

# Common
```
<conbody> the body of the concept topic
<p> a paragraph
<ul> an unordered or bulleted list
<ol> an ordered or numbered list
<sli> simple list
<li> a list item inside a <ul> or <ol>
<fig> a figure, including an optional title
<image> a graphic inside a figure, or inline in text
<section> a subdivision in the topic, with an optional title
	<title> heading, under which you can use the same elements allowed inside the <conbody> element, excluding another <section> element, an <example> element, or a <conbodydiv> element
<related-links> end of topic links
	<link href="URL" format="html" scope="external">
```
# Text Formatting
```
<b> bold text
<i> italic text
<u> underlined text

<sub> subscript text
<sup> superscript text
```

# References & Definitions
```
<xref> cross-references
<note conref="location.dita#topicid/whatduckslike"/> conref to reference content
<fn> Footnote
<dl> List of terms and definitions, presented in a format similar to a two-column table
	<dlentry> definition entry element
	<dt> definition term
	<dd> full definition
<term> a word or phrase that needs a definition
<cite> a word or phrase that needs a citation
<varname> a word or phrase that may change based on the user’s circumstances
```

# Tables
```
<simpletable>
	<sthead> header row
	<strow> body row
	<stentry> simple table entry
<table>
	<title> title for the table
	<tgroup> columns specifications, header rows and body rows
		<colspec> column widths and identifying info
		<thead> table header rows
		<tbody> table body rows
	<row> single row
	<entry> data for table cell
```

# Prolog Elements
```
<author> the content author
<critdates> critical dates, such as <created> and <revised>
<copyright> copyright year <copyryear>, and copyright holder <copyrholder>
<vrm> product version, release, and modification information
```

# Strict Task Topic
```
<taskbody> the body of the task topic
<steps> the sequence of actions
<step> each individual action
	<cmd> the action the user takes; this is a required element in a <step>
	<info> additional information about the step
	<stepresult> what happens after performing an action
	<stepxmp> an example of how to do the step
<example> an example of how to do the entire task
```

# Reference Topic
```
<refbody> the body of the reference topic
<section> a subdivision in the reference topic, with an optional title
<table> a table
<fig> a figure, including an optional title
<properties> a list of properies
<refsyn> a syntax diagram
```

# Glossary Topic
```
<glossentry> the glossary entry topic type
<glossterm> the word or phrase
<glossdef> the definition of the glossary term
```

# Note Types
```
<note>
<attention>
<danger>
<caution>
<important>
<tip>
```

# Other
```
<menucascade> order of a menu path, such as File > Save As
	<uicontrol> text for a menu item
<draft-comment> comments and questions inserted into content while it is being developed
<required-cleanup> wrap content that is tagged incorrectly and needs to be fixed
```

Looking for something else?  
[OxygenXML - DITA Elements, A to Z][oxygen-elements]

[oxygen-elements]: https://www.oxygenxml.com/dita/1.3/specs/langRef/quick-reference/all-elements-a-to-z.html
