---
title: '{{ replace .File.ContentBaseName "-" " " | title }}'
date: {{ .Date }}
draft: true # Change to `false` to publish the page
description: '' # Use to customise the meta description within the head element
slug: '{{ .File.ContentBaseName | urlize }}'
---