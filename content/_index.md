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
 # - block: collection
  #  id: featured
  #  content:
   #   title: Other publications
    #  filters:
     #   folders:
      #    - outreach
       # featured_only: true
  #  design:
   #   columns: '2'
    #  view: card
  - block: experience
    content:
      title: Academic experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Postdoctoral researcher
          company: Universitat Pompeu Fabra
          company_url: ''
          company_logo: ''
          location: Barcelona
          date_start: '2025-02-03'
          date_end: ''
        - title: Postdoctoral researcher
          company: Universitat de Barcelona
          company_url: ''
          company_logo: Logotip_UB
          location: Barcelona
          date_start: '2024-04-14'
          date_end: '2025-01-31'
        - title: Ph.D. researcher
          company: Universitat de Barcelona
          company_url: ''
          company_logo: Logotip_UB
          location: Barcelona
          date_start: '2021-09-01'
          date_end: '2024-04-17'
          #description: |2-
           #   Responsibilities include:

            #  * Analysing
             # * Modelling
              # * Deploying
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
      email: luis.remiro@upf.edu
    #  phone: 888 888 88 88
    #  appointment_url: 'https://calendly.com'
      address:
        # street:
        city: Barcelona
        region: Catalonia
        # postcode:
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