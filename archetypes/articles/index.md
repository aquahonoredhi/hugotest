---
title: '{{ replace .File.ContentBaseName "-" " " | title }}'
date: {{ .Date }}
draft: true # Change to `false` to publish the page
description: '' # Use to customise the meta description within the head element
slug: '{{ .File.ContentBaseName | urlize }}'
summary: '' # An optional summary of the page content
weight: # Use to order the page within the collection, must be an integer, e.g. 0, 1, 2, etc
params:
  author: '' # Name of the person who wrote the article
  tags: ['', ''] # How you’d categorise the article, e.g. Opinion, School News, Lifestyle, etc
  cover:
    image: "cover.jpg"
    alt: "Cover image for {{ replace .Name "-" " " | title }}"
---