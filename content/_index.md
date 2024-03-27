---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: features
    content:
      title: Skills
      items:
        - name: R
        #  description: 100%
          icon: r-project
          icon_pack: fab
        - name: Statistics
         # description: 100%
          icon: chart-line
          icon_pack: fas
        - name: Political science
        #  description: 10%
          icon: check-to-slot
          icon_pack: fas
  - block: collection
    id: publications
    content:
      title: Peer-Reviewed Publications
      #text: |-
       # {{% callout note %}}
        #Quickly discover relevant content by [filtering publications](./publication/).
        #{{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: featured
    content:
      title: Other publications
      filters:
        folders:
          - outreach
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Ph.D. researcher
          company: Universitat de Barcelona
          company_url: ''
          company_logo: Logotip_UB
          location: Barcelona
          date_start: '2021-09-01'
          date_end: ''
          #description: |2-
           #   Responsibilities include:

            #  * Analysing
             # * Modelling
              # * Deploying
        - title: Project information manager
          company: Telematel
          company_url: ''
          company_logo: 'logo_telematel'
          location: Barcelona
          date_start: '2021-02-01'
          date_end: '2021-08-31'
          description: |2-
              Responsibilities include:

              * Data analysis
              * Data management
              * Project management
        - title: Data analyst
          company: Agencia Catalana de Turisme
          company_url: 'https://act.gencat.cat/'
          company_logo: ''
          location: Barcelona
          date_start: '2020-04-01'
          date_end: '2021-01-31'
          description: |2-
              Responsibilities include:

              * Data analysis
              * Public policy design
              * Data visualization
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact me
      subtitle:
      text: |-
        Please, fell free to contact me for more information
      # Contact (add or remove contact options as necessary)
      email: lremiro@ub.edu
    #  phone: 888 888 88 88
    #  appointment_url: 'https://calendly.com'
      address:
        street: Av. Diagonal, 684
        city: Barcelona
        region: Catalonia
        postcode: '08034'
        country: Spain
        country_code: ES
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/LuisMRemiro'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
    design:
      columns: '2'
---