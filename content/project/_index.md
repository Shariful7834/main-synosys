---
title: Projects
date: 2025-04-09

type: landing

sections:
  - block: hero
    content:
      title: "Current and past projects"
      text: ""
    design:
      background:
        image:
          filename: "sharing.png" # Place this in assets/media/
        darken: true
        size: cover
        position: center
      alignment: center
      text_color_light: true

  - block: collection
    content:
      title:
      text: ""
      count: 100
      filters:
        category: ""
        tag: ""
        publication_type: ""
      order: desc
      page_type: project
    design:
      view: Card
      columns: "1"
      text_color_light: true # ✅ Makes title and text white
---
