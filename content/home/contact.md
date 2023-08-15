---
# An instance of the Contact widget.
widget: contact

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 130

title: Contact
subtitle: Write a Brief Message

content:
  # Automatically link email and phone or display as text?
  autolink: true

  # Email form provider
  form:
    provider: netlify
    formspree:
      id:
    netlify:
      # Enable CAPTCHA challenge to reduce spam?
      captcha: true

  # Contact details (edit or remove options as required)
  email: dr [dot] varun [dot] gupta [@] outlook [DOT] com
  address:
    city: Atlanta Metro
    region: Georgia
    country: United States
    country_code: US
  appointment_url: 'https://calendly.com/varunguptaus'
  contact_links:
    - icon: linkedin
      icon_pack: fab
      name: Connect With Me
      link: 'https://www.linkedin.com/in/drvarungupta/'

design:
  columns: '2'
---
