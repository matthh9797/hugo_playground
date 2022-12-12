---
title: "Lesson: Shortcodes"
date: 2022-12-12T10:25:04+07:00
draft: true
author: "Hendo"
---

{{< youtube 2xkNJL4gJ9E >}}

## Notes

 - Shortcodes are HTML "snippets" that you can add into your markdown files

## Types of shortcodes

Shortcodes written in html require further rendering. These can be marked with the surrounding `<>` tags. Shortcodes written in md do not need further rendering, these are surrounded by `%%` tags.

This shortcode is written in *html*: 
{{< test1 "Hello World from HTML!" >}}

This shortcode is written in *markdown*:
{{% test2 "Hello world from markdown" %}}

## Built in shortcodes

A full list of built-in shortcodes can be found [here](https://gohugo.io/content-management/shortcodes/#using-shortcodes)