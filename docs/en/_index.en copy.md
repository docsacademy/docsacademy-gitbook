---
title: "DITA elements"
date: 2023-02-09T11:02:05+06:00
lastmod: 2023-02-09T11:02:05+06:00
weight: 1
draft: false
# search related keywords
keywords: ["elements"]
---

DITA defines its own set of tags called elements. Elements in DITA are used to semantically shape content.
For example, the **section** element is used for sections, and **image** is used for graphical images. Some
of the tags used in DITA are familiar from HTML:

* **p** for paragraphs
* **ol** for ordered lists
* **ul** for unordered lists

The root element in DITA differs depending on the type of topic:

* **concept** for concepts
* **task** for procedures
* **reference** for reference information

DITA elements have their own hierarchy and are connected to each other in a special way. For each element, a set
of elements is defined that may contain this element or that may be contained in this element. In addition, DITA
specifies in what sequence the elements should follow each other and how many elements may be used.

For example, a simple table **simpletable** can have a header followed by one or more standard table cells. Thus,
one of the following situations will be considered a violation:

* The header is in the middle of the table.
* There are no standard cells in the table.