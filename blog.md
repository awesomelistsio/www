---
layout: default
title: Blog
---

<section class="hero">
<div class="hero-inner">
<div>
<div class="hero-pill">Blog</div>
<h1>Insights & Updates</h1>
<p>
Thoughts, updates, and curated insights related to Awesome Lists, open knowledge, software development, AI, security, and digital infrastructure.
</p>
</div>
</div>
</section>

<div class="page-shell">

<section class="panel">

<!--
<div class="section-header">
<div>
<div class="section-label">Latest Posts</div>
<h2>From the blog</h2>
</div>
</div>
-->

<div class="lists-grid">
{% for post in site.posts %}
<article class="card">
<div class="card-top">
<div>
<h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
</div>
</div>

<div class="description">
{{ post.description | strip_html }} <a class="open-link" href="{{ post.url | relative_url }}">
Read
<span class="material-symbols-rounded">
arrow_forward
</span>
</a>
</div>


</article>
{% endfor %}
</div>

</section>

</div>
