---
title: "Learning Hugo"
date: 2022-12-11T11:18:54+07:00
draft: true
author: "Hendo"
language: "English"
tags: ["tag1", "tag2", "tag3"]
categories: ["cat1"]
lessons: ["1"]
---

## Front matter

How do you access front matter?

You can access front matter like so:

```
{{if .Params.language}}Language: {{.Params.Language}}{{end}}
```