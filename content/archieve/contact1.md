---
title: Contact
date: 2024-10-05

type: landing

sections:
  - block: contact
    content:
      title: Contact
      text: |-
        일정을 잡으시려면 이용해주세요
      email: test@example.org
      phone: 888 888 88 88
      address:
        street: 567 Baekje-daero
        city: Jeonju-si
        region: CA
        postcode: '54896'
        country: South Korea
        country_code: KR
      coordinates:
        latitude: '35.847408'
        longitude: '127.130051'
      office_hours:
        - 'Monday 10:00 to 13:00'
        - 'Wednesday 09:00 to 10:00'
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

  - block: markdown
    content:
      title:
      subtitle: ''
      text:
    design:
      columns: '1'
      background:
        image: 
          filename: contact.jpg
          filters:
            brightness: 1
          parallax: false
          position: center
          size: cover
          text_color_light: true
      spacing:
        padding: ['20px', '0', '20px', '0']
      css_class: fullscreen
---