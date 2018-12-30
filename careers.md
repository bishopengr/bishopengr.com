---
title: Careers
permalink: /careers/
---

![](/assets/img/careers.jpg)

Bishop Engineering is a local Civil Engineering and Surveying firm in the western suburbs of Des Moines. We are currently in our 48th year of operation and continue to grow and expand our areas of work each and every year. We specialize in land development including both subdivision design and commercial properties. We also have a large survey department to both support the engineering side of the business and perform several different types of property surveys including ALTA and Site Surveys.

---

## Job Openings

{% if site.jobs.size == 0 %}

There are currently no openings. For inquiries please contact [jabishop@bishopengr.com](mailto:jabishop@bishopengr.com).
{% endif %}

{% for job in site.jobs %}

<h3>{{job.title}}</h3>
{{job.content | markdownify}}

<script type="application/ld+json"> {
  "@context" : "http://schema.org/",
  "@type" : "JobPosting",
  "title" : "{{job.title}}",
  "description" : "{{job.description | markdownify}}",
  "datePosted" : "{{job.datePosted}}",
  "validThrough" : "{{job.validThrough}}",
  "employmentType" : "{{job.employmentType}}",
  "hiringOrganization" : {
    "@type" : "Organization",
    "name" : "{{site.title}}",
    "sameAs" : "{{site.url}}",
    "logo" : "{{site.url}}/assets/img/bishoplogo_large.jpg"
  },
  "jobLocation": {
  "@type": "Place",
    "address": {
    "@type": "PostalAddress",
    "streetAddress": "{{site.streetAddress}}",
    "addressLocality": "{{site.addressLocality}}",
    "addressRegion": "{{site.addressRegion}}",
    "postalCode": "{{site.postalCode}}",
    "addressCountry": "US"
    }
  },
}
</script>

{% endfor %}

## Company Description

Bishop Engineering is a growing Des Moines civil engineering firm specializing in private land development and land surveying. Our typical projects include suburban commercial site plans and residential subdivisions located all across Iowa and stretching into surrounding states. Bishop Engineering is comprised of a vibrant group of technical employees that focus on doing high quality work and meeting our client’s needs and schedules. Find out more about Bishop Engineering at [bishopengr.com](http://www.bishopengr.com "Bishop Engineering")
