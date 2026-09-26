---
title: "{{ replace .Name "-" " " | title }}"
subtitle: "Brand Identity & Design"
date: {{ .Date }}
thumb_image: "images/work-branding-1-thumb.jpg"
thumb_image_alt: "Project preview"
layout: project
sections:
  - type: image_section
    image: "images/work-branding-1.jpg"
    image_alt: "Project imagery"
    caption: ""
    width: wide
  - type: text_section
    content: >-
      Project overview and creative approach.
seo:
  title: "{{ replace .Name "-" " " | title }} | AJU studio"
  description: ""
---
