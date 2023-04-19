---
title: "DITA topics"
date: 2023-02-10T11:02:05+06:00
lastmod: 2023-02-10T11:02:05+06:00
weight: 2
draft: false
# search related keywords
keywords: ["topics"]
---

The basic unit of information in DITA is a topic. Each topic describes only one subject / answers only
one question. Created topics can be used and reused in several documents in a different order.

DITA topics are organized into so-called maps, similar to the table of contents of a book. In maps, you
can specify the sequence of topics and their hierarchy.

The following principles should guide the creation of topics:

* One topic covers only one subject / answers only one question.
* A topic contains enough information to be an independent unit of information.
* A topic is not context-sensitive. This means that the information preceding or following the topic,
is irrelevant.
* One file contains only one topic.

To be valid, a topic must contain at least a root element with an id attribute and a **title** element,
for example:

```html
<topic id="creation">
   <title>Creating a net topic</title>
</topic>
```

### DITA classes

All topics in DITA belong to specific classes. By default, the DITA standard has four types of topics:

* **Topic-concept** contains conceptual information and answers the question **Why**?
* **Topic-Task** contains operational instructions and answers the question **How**?
* **Topic Help** contains background information and answers the question **What**?
* **Vocabulary Topic** contains a description of the term and answers the question **What does it mean**?

Each type of topic is designed to create specific content. Depending on the type of topic, the set of
elements allowed to be used differs.

```html
<topic id="example">
   <shortdesc>Brief topic description</shortdesc>
   <title>Topic title</title>
   <body>This is a container for other elements.</body>
</topic>
```

The root element with the **id** attribute and the **title** element are the only mandatory elements
that must be contained in any topic. Element **shortdesc** contains a brief description of the topic.
The name of element **body**, which contains most of the other elements, varies depending on the type
of the topic. For example, in the task topic the **taskbody** element is used.