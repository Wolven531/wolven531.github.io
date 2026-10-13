---
layout: page
title: Mobile Privacy Policy
permalink: /mobile-privacy-policy/
---

The privacy policy is simple: no personal data shared with us will be given to any third party, under any circumstances. Your data will also never be used by us for any purpose without specific permission.

The app engages in no ad targeting, data mining, or other activities that may compromise your privacy, and we do not affiliate ourselves with any third parties that do so.

## App-specific privacy policies

{% assign studio = site.data.privacy.studio %}{% if studio.play_developer_name == studio.legal_name %}The apps listed below are published on Google Play under the developer name {{ studio.play_developer_name }}, which is also the legal entity responsible for them, and each has its own privacy policy:{% else %}The apps listed below are published on Google Play under the developer name {{ studio.play_developer_name }} by {{ studio.legal_name }}, and each has its own privacy policy:{% endif %}
{% for app in site.data.privacy.apps %}{% assign policy_page = site.pages | where: "app_id", app.id | first %}{% if policy_page %}
- [{{ app.app_name }} Privacy Policy]({{ site.baseurl }}{{ policy_page.url }}){% endif %}{% endfor %}

See [all app privacy policies]({{ site.baseurl }}/privacy/).
