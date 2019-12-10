---
title: TeamWork U
layout: default
cta:
  title: "TeamWork U helps students get hired faster"
  email: "buffy@teamworkonline.com"
  subject: "Test subject"
---
{% assign page_data = site.data.posts.teamWorkU[0] %}

{% include mega-header.html %}

<section class="py4">
<div class="container mx-auto flex flex-wrap">

{% assign item = site.data.posts.educatorTestimonial[0] %}

<div class="md-col-6 px4 my4 black flex items-center wow fadeInUp" data-wow-delay="0.2s">
<div class="flex-auto">
<h2 class="oswald my0 h2">{{ item.title }}</h2>
<p class="h5 regular pb2">{{ item.sub_title }}</p>
{% include cta.html inverted=true %}
</div>
</div>
<div class="md-col-5 wow fadeInUp card-shadow my4" data-wow-delay="0.3s">
<div class="bg-black col-12 px2 py3 flex-none" style="background-color: #002244;">
<h3 class="oswald line-height-4 ltr-spacing-2 h4 m0 regular white">{{ item.quote }}</h3>
</div>
<div class="col-12 bg-white px2 py3 flex-auto">
<div class="flex items-center">
<div class="mr2 flex-none" style="background-image: url({{ item.image.url }}); background-size: cover; background-repeat: no-repeat; background-position: center; height: 64px; width: 64px;"></div>
<div class="flex-auto">
<p class="line-height-1 h5 regular mt0 mb1 black semibold">{{ item.name }}</p>
<p class="line-height-4 h5 regular m0 muted">{{ item.desc }}</p>
</div>
</div>
</div>
</div>

</div>
</section>

<section class="bg-gray">
<div class="container mx-auto py4" style="margin-top: 8rem;">
<div class="flex flex-wrap" style="margin-top: -8rem;">
{% assign benefits = site.data.posts.benefits | sort: 'sort' %}
{% for item in benefits %}
<div class="flex-auto col-4 mx2 px3 pt3 card-shadow bg-white">
<h2 class="oswald black mb3 center">{{ item.title }}</h2>
<div class="pb3">
<ul>
<li><h3 class="line-height-5 regular black checkmark">{{ item.ben1 }}</h3></li>
<li><h3 class="line-height-5 regular black checkmark">{{ item.ben2 }}</h3></li>
<li><h3 class="line-height-5 regular black checkmark">{{ item.ben3 }}</h3></li>
</ul>
</div>
</div>

{% endfor %}
</div>
</div>
</section>

<section class="py4">
<div class="container mx-auto flex flex-wrap">
<h2 class="oswald black mb3 center">Calculator</h2>
</div>
</section>

<section class="py4">
<div class="container mx-auto flex flex-wrap">

{% assign item = site.data.posts.schools[0] %}

<div class="md-col-6 px4 my4 black flex items-center wow fadeInUp" data-wow-delay="0.2s">
<div class="flex-auto">
<h3 class="oswald h3">{{ item.title }}</h3>
{% include cta.html inverted=true %}
</div>
</div>

<div class="px2 col-12 md-col-8 mx-auto">
<div class="flex flex-wrap my3">
  {% for item in item.image %}
  <div class="col-6 md-col-3 center px2 mt2">
    <img class="inline-block mb1" src="{{ item.url }}" alt="{{ item.title }}" width="100" />
  </div>
  {% endfor %}
</div>
</div>

</div>
</section>

<section class="py4">
<div class="container mx-auto flex flex-wrap">

{% assign item = site.data.posts.studentTestimonial[0] %}

<div class="md-col-6 px4 my4 black flex items-center wow fadeInUp" data-wow-delay="0.2s">
<div class="flex-auto">
<h2 class="oswald my0 h2">{{ item.title }}</h2>
<p class="h5 regular pb2">{{ item.sub_title }}</p>
{% include cta.html inverted=true %}
</div>
</div>

<div class="md-col-5 wow fadeInUp card-shadow my4" data-wow-delay="0.3s">
<div class="bg-black col-12 px2 py3 flex-none" style="background-color: #002244;">
<h3 class="oswald line-height-4 ltr-spacing-2 h4 m0 pb2 regular white">{{ item.quote }}<i class="icofont-dart icofont-1x"></i></h3>

<a href="{{ item.url }}" target="new" class="oswald white" style="text-decoration: none;"><img src="/images/youtube-play.svg" width="24px;" class="mr1 pt1">{{ item.cta }}</a>
</div>

<div class="col-12 bg-white px2 py3 flex-auto">
<div class="flex items-center">
<div class="mr2 flex-none" style="background-image: url({{ item.image.url }}); background-size: cover; background-repeat: no-repeat; background-position: center; height: 64px; width: 64px;"></div>
<div class="flex-auto">
<p class="line-height-1 h5 regular mt0 mb1 black semibold">{{ item.name }}</p>
<p class="line-height-4 h5 regular m0 muted">{{ item.desc }}</p>
</div>
</div>
</div>
</div>

</div>
</section>
