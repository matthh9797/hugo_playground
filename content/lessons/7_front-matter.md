---
title: "Learning Hugo"
date: 2022-12-11T11:18:54+07:00
draft: false
author: "Hendo"
language: "English"
section: ["Front matter"]
---

## Front matter

How do you access front matter?

You can access front matter like so:

```
{{if .Params.language}}Language: {{.Params.Language}}{{end}}
```
