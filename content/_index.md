---
# Leave the homepage title empty to use the site title
title:
date: 2025-01-07
type: landing

sections:
  - block: markdown
    content:
      title: ""
      subtitle: ""
      text: |
        <div class="mw-max center cf white tl">
          <div class="w-50 fl pa0 ma0">
            <img src="SynoSys_logo_png_combine.png" alt="SynoSys Logo" class="w-90 p-8"> 
            <div class="tl f1-l f4-m f4 fw6">
              The Center Synergy of Systems
            </div>
            <div class="f2-l f4-m f4 tr mt5-l mt2 pa4" style="--duration: 1.8s; --delay: 0s">
              <span class="animate_me" style="font-size: 2.2vw;font-weight:300; max-width: 100%;">
                "We get lost in Science!"
              </span>
            </div>
          </div>
          <div class="w-50 fl tc mt5-ns mt1-m mt1" id="animation"></div>
          <script src="https://cdn.jsdelivr.net/npm/synosys_site_visualization@1.1.4"></script>
          <script>
            synosys_site_visualization.load("animation");
          </script>
        </div>

    design:
      background:
        # image:
        #   filename: "background_banner.jpg"
        #   position: right
        #   size: cover
        text_color_light: true

        image_darken: 1
        color: "#000"

  - block: youtube
    content:
      title: "Creed for Complexity"
      text: |
        <div class="titillium-web-extralight" style="text-align: justify; line-height: 1.4; font-size:1.2rem ">
        SynoSys is Complexity Science. The spirit and perspectives that Complexity Science offers pervade the Center, its people and their activities. 
        We investigate phenomena that seem unrelated at first glance. Yet, we seek and search for underlying rules that connect them. 
        We have an anti-disciplinary attitude, we are neo-generalists, we transcend the borders of traditional disciplines. We explore, 
        we do science with a compass, rather than a map. We get lost in science.</div>
      video_id: "-9VLMfnXtS4"

    design:
      background:
        gradient_start: "#dbd9d9"
        gradient_end: "#ebe8e8"
        text_color_light: false

  # - block: hero
  #   content:
  #     text: |
  #       The central research questions are: How is public discourse shaped by social networks and sorting algorithms, and how does it benefit certain rhetoric? How do generated images affect attention and emotions and how do they reinforce certain narratives more than others? Establishing causality between these factors in such complex socio-technical systems is an overarching challenge that we aim to address.
  #       <br>
  #       To achieve this, we are convinced that looking at those systems from various angles is crucial. While the overarching questions span the whole research groups, we are composed of a variety of disciplinary backgrounds and methods. Digitalization is not only impacting social systems, but also expanding the methods for studying them and enabling us to cover a spectrum of measurements of human behavior between micro and macro levels, ranging from online experiments to field studies in social media and large-scale platform data analysis, while computer simulations may help connect the scales.

  - block: people
    id: people # Add this line to create an anchor ID
    content:
      title: Meet the Team
      user_groups:
        - Principal Investigators
        - Members
        - Grad Students
        - Administration
        - Visitors
        - Alumni
      sort_by: Params.last_name
      sort_ascending: true
    design:
      show_interests: false
      show_role: true
      show_social: true

  - block: collection
    id: news # Add this line to create an anchor ID
    content:
      title: Latest News
      subtitle:
      text:
      count: 15
      filters:
        author: ""
        category: ""
        exclude_featured: false
        publication_type: ""
        tag: ""
      offset: 0
      order: desc
      page_type: post
    design:
      view: Card
      columns: "1"

  # - block: markdown
  #   content:
  #     title:
  #     subtitle: ""
  #     text:
  #   design:
  #     columns: "1"
  #     background:
  #       image:
  #         filename: coders.jpg
  #         filters:
  #           brightness: 1
  #         parallax: false
  #         position: center
  #         size: cover
  #         text_color_light: true
  #     spacing:
  #       padding: ["20px", "0", "20px", "0"]
  #     css_class: fullscreen

  # - block: collection
  #   content:
  #     title: Latest Preprints
  #     text: ""
  #     count: 5
  #     filters:
  #       folders:
  #         - publication
  #       publication_type: "article"
  #   design:
  #     view: citation
  #     columns: "1"

  # - block: markdown
  #   content:
  #     title:
  #     subtitle:
  #     text: |
  #       {{% cta cta_link="./people/" cta_text="Meet the team →" %}}
  #   design:
  #     columns: "1"
---
