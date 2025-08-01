---
_schema: default
draft: false
eleventyExcludeFromCollections: false
disableNav: false
disableSitemap: false
title: 'Book Editing '
metaDesc:
customCode:
  headCode: ''
  bodyCode: ''
serviceImage: /assets/uploads/1346.jpg
imageAltText:
category:
summary:
pageLink: Book-Editing-Service
permalink: >-
  /services/{% capture varPagePath %}{% if pageLink%}{% assign pageLink =
  pageLink | slugify%}{{  page.filePathStem |fileSubstringFilter | append:
  pageLink }}{% else %}{% assign title = title | slugify%}{{  page.filePathStem
  |fileSubstringFilter | append: title }}{% endif %}{% endcapture
  %}/{{varPagePath | strip}}/index.html
layout: layouts/page.html
id: c422e79a-0475-4a7a-85a6-c6d66f3fae1f
hero:
content_blocks: []
_inputs:
  headCode:
    type: code
    comment: Add code at the end of the <head> tag
  bodyCode:
    type: code
    comment: Add code before the </body> tag
---
