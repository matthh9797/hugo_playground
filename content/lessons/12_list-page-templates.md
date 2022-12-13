---
title: "Lesson: 12_list Page Templates"
date: 2022-12-13T09:52:29+07:00
draft: true
author: "Hendo"
section: ["Templates"]
---

{{< youtube 8b2YTSMdMps >}}

## Notes

 - You can overwrite the default list page in a section by including an _index.md file.
 - To change the default pages, in layouts folder create a new file. (For example layouts/_default/list.html changes the default list page) 

## How to list content

You can loop over the pages and there variables by using something like:

```
{{ range .Pages }}
    {{.Title}} - {{.RelPermalink}} <br>
{{end}}
```

 - range is a for loop for hugo
 - .Pages access the pages which belong to this section
 - .Title is the specific pages title
 - .RelPermalink Relative permanent link to a page

For a full list of page variables look [here](https://gohugo.io/variables/page/)

 Below is the full html code to list pages in a section and link to this pages:

 ```
<html>
<head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <meta http-equiv="X-UA-Compatible" content="ie=edge">
     <title>Document</title>
</head>
<body>
    {{.Content}}
    {{ range .Pages }}
        <ul>
            <li><a href="{{.RelPermalink}}">{{.Title}}</a></li>
        </ul>
    {{end}}
</body>
</html>
 ```