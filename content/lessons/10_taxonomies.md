---
title: "Lesson: 10_taxonomies"
date: 2022-12-13T08:17:56+07:00
draft: true
author: "Hendo"
section: ["Taxonomies"]
---

{{< youtube pCPCQgqC8RA >}}

## Notes

 - Taxonomies are how to group content together. These are site wide entities and therefore custom taxonomies need specified in the config file.

By default Hugo provides two taxonomies:
 - Tags 
 - Categories 

 - Taxonomies are added in the front matter of the content files
 - Hugo will create a page for specific taxonomies. But if not a default taxonomy you will need to add the following line to your config.toml

```
[taxonomies]
    mood = "moods"
```

You will also need to add a line to your html code if you would like the section to show on list and single pages. For example:

```
<div>{{ if .Params.section }}<strong>Section:</strong> {{range .Params.section}}<a href="{{ "/section/" | relLangURL }}{{ . | urlize }}">{{ . }}</a> {{end}}{{end}}</div>
```

## Real life examples of taxonomies

 - Music genres
 - Species
 - Moods