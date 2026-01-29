---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Education

**Ph.D. in Computer Science** (Expected December 2028)  
Louisiana State University, Baton Rouge, LA  
*Research Focus: Program Analysis, Formal Methods, Android Security*

## Research Experience

**Graduate Research Assistant** | Louisiana State University  
*2023 - Present*

- Developed static analysis techniques for Android application security
- Published research on Android Auto app compliance violations
- Working on taint analysis using SootUp and FlowDroid
- Exploring supply chain security research for Android/JVM ecosystems

## Publications

{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}

## Technical Skills

**Programming Languages**: Java, Python, Kotlin  
**Static Analysis Tools**: SootUp, FlowDroid, Soot  
**Distributed Systems**: Apache Spark, Hadoop, Google Cloud Dataproc  
**Development Tools**: Docker, Git, tree-sitter  
**Areas of Expertise**: Android Development, Taint Analysis, Program Verification

## Teaching

{% for post in site.teaching reversed %}
  {% include archive-single-cv.html %}
{% endfor %}

## Service & Leadership

- Contributor to Thunderbird Android
- Peer reviewer for software engineering venues
