
---
layout: default
title: About Me
---

<header>
  <h1>About Me</h1>
</header>

<article class="post h-entry" itemscope itemtype="http://schema.org/BlogPosting">

  <header class="post-header">
    <h1 class="post-title p-name" itemprop="name headline">{{ page.title | escape }}</h1>
    <p class="post-meta">
      <time class="dt-published" datetime="{{ page.date | date_to_xmlschema }}" itemprop="datePublished">
        {%- assign date_format = site.minima.date_format | default: "%b %-d, %Y" -%}
        {{ page.date | date: date_format }}
      </time>
      {% assign author = page.author | default: site.author %}
      {%- if author -%}
        • <span itemprop="author" itemscope itemtype="http://schema.org/Person"><span class="p-author h-card" itemprop="name">{{ author }}</span></span>
      {%- endif -%}</p>
  </header>

  <div class="share-links">
    {% include sharelinks.html %}
  </div>

  <div class="post-content e-content" itemprop="articleBody">
    <p>Hi there, this is my blog and here I will showcase things revolving around Cyber Security, things I've seen in the field and anything else I see fit.</p>
    
    <p>My name is Logan Crabtree and I have been in the cyber field for almost a year now. I was an intern pentester for AEP, with a focus on red teaming (obviously) in Web Development. It was quite fun but unfortunately, it had to come to an end. I want to work in all fields of cyber security eventually but my dream job is to be a physical pentester. I have started learning how to lockpick and from time to time I practice social engineering.</p>
    
    <p>My journey has been a bumpy one but I'm keeping my head down and grinding out what I need to. I started college in 2020 right out of high school but I took some detours along the way. I am currently almost done with school; graduating this year. So that's a little bit about me.</p>
    
    {% include navlinks.html %}
  </div>

  <a class="u-url" href="{{ page.url | relative_url }}" hidden></a>
</article>

