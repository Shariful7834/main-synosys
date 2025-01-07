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
      text: >
        <div class="mw-max center cf white tl">
          <div class="w-80 fl mt5-ns mt1-m mt1 pa3">
            <div class="f-headline-l lh-title f1-m f1 mb0 mb2-ns">Computational Social Science</div>
            <div class="baskerville tl f1-l f4-m f4">Research on the Complex Interaction between Digitalization and Society <br> @ SynoSys</div>
            </div>
          </div>
          <div class="w-50 fl tc mt5-ns mt1-m mt1" id="animation">
          </div>
          <script src="https://cdn.jsdelivr.net/npm/synosys_site_visualization@1.1.3"></script>
        </div>
    design:
      background:
        image:
          filename: "sketch.jpeg"
          position: bottom
          size: cover
        text_color_light: true
        image_darken: 0.4

  - block: hero
    content:
      #title: |
      #  Unraveling complexities of the online environment
      image:
        filename: landing.png
      text: 
        Digitalization has transformed our information environments and social world, giving rise to a complex system with many-to-many interactions. Online platforms such as social media and search engines have created new degrees of freedom while also introducing new constraints, such as the algorithmic curation of content. Meanwhile, generative AI has expanded the means and scope of content production, all of which is almost constantly accessible via smartphones. These developments have changed the nature of public discourse, shifted roles and power, and are affecting democratic systems around the world.
       

  - block: hero
    content:

      text: |
        The central research questions are: How is public discourse shaped by social networks and sorting algorithms, and how does it benefit certain rhetoric? How do generated images affect attention and emotions and how do they reinforce certain narratives more than others? Establishing causality between these factors in such complex socio-technical systems is an overarching challenge that we aim to address. 
        <br>
        To achieve this, we are convinced that looking at those systems from various angles is crucial. While the overarching questions span the whole research groups, we are composed of a variety of disciplinary backgrounds and methods. Digitalization is not only impacting social systems, but also expanding the methods for studying them and enabling us to cover a spectrum of measurements of human behavior between micro and macro levels, ranging from online experiments to field studies in social media and large-scale platform data analysis, while computer simulations may help connect the scales.




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
