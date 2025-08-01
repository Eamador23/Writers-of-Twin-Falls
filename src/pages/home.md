---
_schema: default
draft: false
title: Home
eleventyExcludeFromCollections: false
disableNav: false
disableSitemap: false
removeFromNavigation: false
eleventyNavigation:
  key: Home
  order: 1
  title:
  parent:
  url:
pageLink: /
permalink: >-
  {% if pageLink == 'blog' or pageLink == 'Blog' %}/{{pageLink | slugify}}{% if
  pagination.pageNumber > 0 %}/page/{{ pagination.pageNumber }}{% endif
  %}/index.html{% elsif pageLink %}/{% assign pagelink = pageLink | slugify
  %}{{  page.filePathStem | fileSubstringFilter | append: pagelink | downcase
  }}/index.html{% else %}/{% assign title = title | slugify %}{{
  page.filePathStem | fileSubstringFilter | append: title | downcase
  }}/index.html{%endif %}
metaDesc:
customCode:
  headCode: ''
  bodyCode: ''
addToCollections: false
layout: layouts/page.html
hero:
  _bookshop_name: sections/fullImageTextBottomHero
  content:
    sectionId:
    highlightEybrow: false
    eyebrow: ''
    headline: Join Writers of Twin Falls
    description: Work on your current writing project and connect with other creatives.
    buttons:
      - _bookshop_name: generic/button
        url: /about-us/
        openInNewTab: false
        text: Learn More About Us
        color_group: 5c9075f8-80f9-4482-b041-91cffdfe02be
        colorFromGroup: primary
        ghostButton: false
        formSubmit: false
    image:
      _bookshop_name: generic/image
      imagePath: /assets/uploads/home/fog-forest.png
      imageAlt: Image of a foggy forest.
      yAxisPosition:
      imageSizes:
      class:
      imageNumber:
  styles:
    color_group: primary
    backgroundOpacity: 55
content_blocks: []
_inputs:
  removeFromNavigation:
    hidden: true
  eleventyNavigation:
    hidden: true
  headCode:
    type: code
    comment: Add code at the end of the <head> tag
  bodyCode:
    type: code
    comment: Add code before the </body> tag
  addToCollections:
    type: switch
    comment: Enabling this allows this page to be added to collections of your choosing
  tags:
    hidden: '!addToCollections'
    type: multiselect
    options:
      values: data.pageCollections.tags[*]
  collectionImage:
    hidden: '!addToCollections'
  imageAltText:
    hidden: '!addToCollections'
  keyInformation:
    hidden: '!addToCollections'
    label: Key information
    comment: >-
      Short description or summary for this page. Will be shown on the
      collection cards
    type: markdown
    options:
      link: true
      blockquote: false
      bold: true
      italic: true
      strike: true
      subscript: true
      superscript: true
      underline: true
      bulletedlist: true
      numberedlist: true
      indent: false
      outdent: false
      code: false
      embed: false
      horizontalrule: false
      image: false
      table: false
      undo: true
      redo: true
      removeformat: true
      copyformatting: true
---
