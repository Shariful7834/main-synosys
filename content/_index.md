---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: markdown
    content:
      title: ""
      subtitle: ""
      text: >
        <div class="mw-max center cf white tl">
          <div class="w-50 fl mt5-ns mt1-m mt1 pa3">
            <div class="f-headline-l lh-title f1-m f1 mb0 mb5-ns">SynoSys</div>
            <div class="baskerville tl f1-l f4-m f4">The Center Synergy of Systems</div>
            <div class="baskerville i f2-l f4-m f4 tr mt5-l mt2" style="--duration: 1.5s; --delay: 0s">
              <span class="dont_animate">"We get lost ...</span>
              <span class="animate_me">in Science!"</span>
            </div>
          </div>
          <div class="w-50 fl tc mt5-ns mt1-m mt1" id="animation">
          </div>
          <script src="https://cdn.jsdelivr.net/npm/synosys_site_visualization@1.1.3"></script>
          <script>
            synosys_site_visualization.load("animation");
          </script>
        </div>
    design:
      background:
        image:
          filename: "background_banner.jpg"
          position: center
          size: cover
        text_color_light: true
        image_darken: 0.4

  - block: hero
    content:
      title: |
        Computational Social Science
      image:
        filename: landing.png
      text: |
        <br>

        Research into the complexity of social systems is represented by the young investigators group. New types of data enable the quantitative description and modelling of social phenomena on a large scale, such as social network structures, public opinion formation, collective behaviour or longitudinal societal; at the same time, digitalization is also changing the mechanisms at work, e.g. through digital communication on social media or algorithmic curation of information. Our aim is to view these systems and developments through the lens of complex systems, but with a strong empirical and experimental perspective from the social sciences.

  - block: people
    id: people # Add this line to create an anchor ID
    content:
      title: Meet the Team
      user_groups:
        - Principal Investigators
        - Researchers
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
      count: 5
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
