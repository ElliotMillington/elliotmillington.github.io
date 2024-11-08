---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/CV_Elliot-Millington.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I am committed to improving the health and wellbeing of neurodivergent people, especially autistic people and those with learning disabilities. My interests span several areas, each addressing different facets of health and healthcare disparities in these populations.

        One focus of my work is the relationship between sensory processing and mental health, particularly how sensory experiences influence anxiety in autistic individuals. This interest began with my PhD research, where I used both experimental and questionnaire methods to explore their bidirectional relationship. Another strand of my work examines how social determinants - such as socioeconomic status and access to public services - affect health outcomes for neurodivergent people. In my current role with the Scottish Learning Disabilities Observatory, I use large administrative datasets to uncover patterns and disparities that shape healthcare access and overall wellbeing for autistic people and those with learning disabilities.
        
        Please reach out to collaborate 😃
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
---
