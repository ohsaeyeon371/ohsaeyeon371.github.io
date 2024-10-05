---
# An instance of the About widget.
# Documentation: https://docs.hugoblox.com/page-builder/
widget: about

# Activate this widget? true/false
active: true

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 10

title: introdution

sections:
  - block: experience
    content:
      title: experience
      text: |-
        Lorem ipsum dolor sit amet
      email: test@example.org
      phone: 888 888 88 88
      address:
        street: 450 Serra Mall
        city: Stanford
        region: CA
        postcode: '94305'
        country: United States
        country_code: US
      coordinates:
        latitude: '37.4275'
        longitude: '-122.1697'
      directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      appointment_url: 'https://calendly.com'
      #contact_links:
      #  - icon: comments
      #    icon_pack: fas
      #    name: Discuss on Forum
      #    link: 'https://discourse.gohugo.io'
    
      # Automatically link email and phone or display as text?
      autolink: true
    
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '1'      

# content:
#     coordinates:
#         latitude: '37.4275'
#         longitude: '-122.1697'

# Choose the user profile to display
# This should be the username (folder name) of a profile in your `content/authors/` folder.
# See https://docs.hugoblox.com/get-started/#introduce-yourself
author: admin
---
