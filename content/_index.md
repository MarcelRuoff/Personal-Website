---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
  - block: features
    content:
      title: Skills
      items:
        - name: Angular
         # description: 90%
          icon: angular
          icon_pack: custom
        - name: Python
         # description: 90%
          icon: python
          icon_pack: custom
        - name: C#
         # description: 70%
          icon: code
          icon_pack: fas
        - name: Natural Language Processing
         # description: 65%
          icon: nlp
          icon_pack: custom
        - name: Data Science
         # description: 65%
          icon: chart-line
          icon_pack: fas
      
 # - block: portfolio
 #   id: projects
 #   content:
 #     title: Projects
 #     filters:
 #       folders:
 #         - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
 #     default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
 #     buttons:
 #       - name: All
 #         tag: '*'
 #       - name: Deep Learning
 #         tag: Deep Learning
 #       - name: Other
 #         tag: Demo
 #   design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
 #     columns: '1'
 #     view: showcase
      # For Showcase view, flip alternate rows?
 #     flip_alt_rows: false
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
        exclude_future: false
    design:
      columns: '1'
      view: showcase  # compact
  - block: collection
    content:
      title: Recent Publications
      count: 5
      text: ''
      filters:
        folders:
          - publication
        exclude_featured: false
        exclude_future: false

    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
      sort_ascending: true
    design:
      columns: '2'
      view: compact
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
      # Contact (add or remove contact options as necessary)
      email: marcelruoff[at]gmx.de
      # Automatically link email and phone or display as text?
      autolink: false
      # Email form provider
      #form:
      #  provider: netlify
      #  formspree:
      #    id:
      #  netlify:
          # Enable CAPTCHA challenge to reduce spam?
      #    captcha: true
    design:
      columns: '2'
---
